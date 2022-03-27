# Linking & Unlinking

{% hint style="info" %}
These commands replace the old `/voice` `/stage` and `/category` commands
{% endhint %}

These commands allow you to link **voice** channels, **category** channels, and **stage** channels.

You can use these commands to link a role that is given on joining, a role that is removed on joining, or a suffix that is added to your username on joining.

## /link

This command is used to create a 'normal' link between a channel and a role. 'Normal' links are when a member is given a role when they join the channel, and it is removed when they leave.

You can create multiple channel-role links per channel, allowing users to be given a selection of roles when they join a channel.

![An example of the /link command](<../../.gitbook/assets/image (12).png>)

{% hint style="warning" %}
The 'VC Roles' role needs to be above the role which you are linking, otherwise, you will not be given the role.
{% endhint %}

## /unlink

This command is the opposite of the [link ](linking-and-unlinking.md#link)command, removing a channel-role link. After removing the link, members will not be given roles when they join the channel.

![An example of the /unlink command](<../../.gitbook/assets/image (13).png>)

## /suffix \[add/remove]

This command is used to link a suffix to a channel. When a member joins the channel, the suffix will be added to their username, and when they leave the suffix will be removed.

E.g. your name before joining could be: `cde` and when you join: `cde | ONLINE` if the suffix was `| ONLINE`

![/suffix add command](<../../.gitbook/assets/image (7).png>)

![/suffix remove command](<../../.gitbook/assets/image (27).png>)

## /reverse \[link/unlink]

These commands are used to create a reverse channel-role link. Unlike the 'normal' link the reverse link removes the role when the member joins and adds it when they leave.

![/reverse link command](<../../.gitbook/assets/image (14).png>)

![/reverse unlink command](<../../.gitbook/assets/image (15).png>)
