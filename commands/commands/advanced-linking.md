# Advanced Linking

{% hint style="info" %}
This feature can be quite complicated to understand but is a powerful tool when mastered.
{% endhint %}

Advanced linking allows you to link or unlink many channels with a single command, even allowing for creating new channels or roles.



This feature can be used in many ways, but one such way could be setting up an entire server instantly with voice channels & linking them instantly, without individually using the commands

## /advanced

To use this command, you first need a valid JSON file for the bot. The bot will read this file, and update the linked channels for your guild.

Read the [Making a JSON file guide](advanced-linking.md#making-a-json-file) below for help

## /export

This command will return all the linked channels in your guild in a format that is compatible with the [/advanced](advanced-linking.md#advanced) command

## Making a JSON file

The process of making a file for the [/advanced](advanced-linking.md#advanced) command can seem complicated at first, so we'll walk you through the basic steps.

For this, you will need a JSON editor to ensure there are no syntax errors. An editor such as VS Code can be used, or an online editor such as [here](https://jsoneditoronline.org/#left=cloud.285817e6d69b42b183d601c08ffd571a). You will also need to be able to download the finished JSON file.

We will start off with this template, which currently will do nothing when used:

```json
{
    "all": {},
    "category": {},
    "permanent": {},
    "stage": {},
    "voice": {}
}
```

### Linking:

In order to add our first link, we must first understand the format the bot expects to receive data in.

With the keys: category, permanent, stage, and voice, the bot will expect data to look like this:

```json
// data format for category, permanent, stage and voice keys
{
    channel: {
        "roles": [role],
        "suffix": "",
        "reverse_roles": [role]
    }
}
```

The key all expects data in a slightly different format as you aren't linking any specific channels, so looks like this:

```json
// data format for 'all' key
{
    "roles": [role],
    "suffix": "",
    "reverse_roles": [role]
}
```

Here, `channel` must be a **string** of either a **channel id** or a **channel name**. If the channel name is given and does not exist already, a new channel will be created.

`[role]` here must be a **list** of items separated by commas with each item as a **string** of either a **role id** or a **role name**, and once again if the role name given does not already exist, a new role will be created.

The `suffix` key just needs a **string** value of the suffix that you wish to link.

```json
// Example with channel/role ids being used:
{
    "951147593793159250": {
        "roles": ["808797479553466438", "808792319788056576"],
        "suffix": "",
        "reverse_roles": ["775471163102462009"]
    }
}
// Example with channel/role names being used:
{
    "Welcome": {
        "roles": ["Members", "Verified"],
        "suffix": "",
        "reverse_roles": ["Unverified"]
    }
}
```

We can now combine the initial template & these examples to link channels:

```json
{
    "all": {
        "roles": ["In Voice Channel"],
        "suffix": "| IN VC"
    },
    "category": {},
    "permanent": {
        "Welcome": {
            "roles": ["Members", "Verified"],
            "suffix": "| MEMBER",
            "reverse_roles": ["Unverified"]
        }
    },
    "stage": {},
    "voice": {
        "951147593793159250": {
            "roles": ["808797479553466438", "808792319788056576"],
            "suffix": "",
            "reverse_roles": ["775471163102462009"]
        }
    }
}
```

### Unlinking:

Unlinking commands follows a similar format, with one key difference: you need to add `!` (an exclamation mark) in front of the role, channel, or entire link-type you want to unlink.

To unlink a single, specific role from a channel, we could use something like this (works the same with reverse\_roles):

```json
"voice/permanent/...": {
        channel: { // channel can be id or name
            "roles": ["!808797479553466438", "!Verified"] // note ! before the role
        }
    }
```

If we wanted to unlink every role or suffix from a channel, we could use something like this:

```json
"voice/permanent/...": {
        channel: { // channel can be id or name
            "!roles": [], // note ! before "roles" & it doesn't matter what the list contains 
            "!suffix" : ""
        }
    }
```

If we wanted to remove every link associated with the channel we could do:

```json
"voice/permanent/...": {
        !channel: {} // note channel must be a str id
    }
```

If we wanted to remove all links of a certain type (e.g. voice) we can use:

```json
"!voice" : {}
```

We can now combine the initial template & these examples to unlink channels:

```json
{
    "all": {},
    "!category": {}, // unlinks all categories
    "permanent": {
        "Welcome": {
            "roles": ["!Members", "!808792319788056576"], // unlinks specific roles
            "!reverse_roles": [] // removes all reverse role links
        }
    },
    "stage": {
        "!951147593793159250": {} // removes all links for stage with id 951147593793159250
    },
    "voice": {
        "951147593793159250": {
            "!roles": [], // removes all role links
            "!suffix": "" // removes linked suffix
        }
    }
}
```

### Final File:

Now we understand both linking & unlinking, we can combine them into a single file that does both.

```json
{
    "!all": {}, // remove all links of type all
    "all": { // create new links of type all
        "roles": [
            "In Voice Channel" // link role by name
        ],
        "suffix": "| IN VC" // link suffix
    },
    "category": {
        "!758392649979265025": {}, // remove all links for specific category
        "758392649979265025": { // create new links for specific category
            "roles": [
                "809387324969451531" // link role by id
            ],
            "suffix": "cat",
            "reverse_roles": [
                "818482958578483301" // reverse link role by id
            ]
        }
    },
    "permanent": {
        "Welcome": { // create new links for permanent channel with name "Welcome"
            "roles": [
                "Members",
                "Verified"
            ],
            "suffix": "| MEMBER", // link suffix
            "reverse_roles": [
                "Unverified"
            ]
        }
    },
    "stage": {
        "944261529908436992": { // create new links for stage channel with id 944261529908436992
            "suffix": "| STAGE 1", // link suffix
            "!roles": [], // remove all linked roles
            "reverse_roles": [
                "!944261529908436992" // remove specific reverse linked role
            ]
        }
    },
    "!voice": {} // remove all linked voice channels
}
```

{% hint style="info" %}
Support with advanced linking can be found in our [support server](https://discord.gg/yHU6qcgNPy)
{% endhint %}
