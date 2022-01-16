# Overview

### [Add to your Discord Server!](https://discord.com/api/oauth2/authorize?client\_id=775025797034541107\&permissions=300944400\&scope=bot%20applications.commands)

[Discord Support Server](https://discord.com/invite/yHU6qcgNPy) | [View Documentation](https://www.vcroles.com) | [View GitHub](https://github.com/CDESamBotDev/VCRoles) | [Top.gg Page](https://top.gg/bot/775025797034541107) | [Patreon Page](https://www.patreon.com/CDESamBots)

## Introduction

Welcome to the VC Roles documentation! Here you'll find everything you need to get up and running with the bot!

If you want to report a bug or request a feature, head over to our [GitHub page](https://github.com/CDESamBotDev/VCRoles/issues), and make a new issue!

### Ready to start?

Jump right into the quick start docs and start setting up the bot right now!

{% content-ref url="basic-setup.md" %}
[basic-setup.md](basic-setup.md)
{% endcontent-ref %}

## Features

VC Roles is a bot that will make your server and its voice channels much more interactive, enabling features such as: giving members roles when they join a voice channel, removing it on leave, reading TTS messages in voice channels, for those without a mic, creating and managing voice channels, and much more!&#x20;

This is the bot you need to make your server more interactive, and bring your community together!

* [Voice Channel - Role linking](commands/commands/voice-linking.md)
  * A role(s) will be given to a member when they join the voice channel, and removed when they leave
  * Great for hiding voice reply channels, or music bot command channels when they aren't needed
* [Category - Role linking](commands/commands/category-linking.md)
  * A role(s) will be given to a member when they join any voice channel in a category, and removed when they leave
* [Stage Channel - Role linking](commands/commands/stage-linking.md)
  * A role(s) will be given to a member when they join the stage channel, and removed when they leave
  * Great for hiding a stage discussion channel so that only those who are in the stage channel can participate
* [All channel - Role linking](commands/commands/all-linking.md)
  * A role(s) will be given to a member when they join any voice channel, and removed when they leave
  * Option to add exception channels (members aren't given the 'all' role(s) when they join/leave)
* [Permanent Role Links](commands/commands/permanent-linking.md)
  * A role(s) will be given to a member when they join the voice channel, and will remain after they leave.
  * Great for easy user verification
* [Voice Admin Commands](commands/commands/voice-admin-commands.md)
  * Used to _(un)_mute/_(un)_deafen all members in a voice channel
* [Voice Channel TTS commands](commands/commands/tts-commands.md)
  * TTS commands are used to make the bot read a message in a voice channel
  * Options for multiple languages.
  * Great for users who have no mic and still want to be heard
* [Voice Channel Generators](commands/commands/voice-channel-generators.md)
  * When a member joins the generator channel a new voice channel is made just for them, and is deleted when there are no more members in the channel.
* [Audit logging (for voice channels)](commands/commands/audit-logging.md)
  * See when members join, leave or change voice channels, and the roles that are given/removed by the bot.
