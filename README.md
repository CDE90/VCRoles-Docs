# Overview

## The website has now changed. For up-to-date information and to use the new web dashboard, please visit our new site: [https://vcroles.com](https://vcroles.com)



















### [Add to your Discord Server!](https://discord.com/api/oauth2/authorize?client\_id=775025797034541107\&permissions=1039166576\&scope=bot%20applications.commands) | [Upgrade to Premium](https://cde90.gumroad.com/l/vcroles)

[Discord Support Server](https://discord.com/invite/yHU6qcgNPy) | [View Documentation](https://www.vcroles.com/) | [View GitHub](https://github.com/CDE90/VCRoles) | [Top.gg Page](https://top.gg/bot/775025797034541107)

{% embed url="https://premium.vcroles.com/l/vcroles" %}

## Introduction

Welcome to the VC Roles documentation! Here you'll find everything you need to get up and running with the bot!

If you want to report a bug or request a feature, head over to our [GitHub page](https://github.com/CDE90/VCRoles), and make a new issue!

### Ready to start?

Jump right into the quick start docs and start setting up the bot right now!

{% content-ref url="basic-setup.md" %}
[basic-setup.md](basic-setup.md)
{% endcontent-ref %}

## Features

VC Roles is a bot that will make your server and its voice channels much more interactive, enabling features such as: giving members roles when they join a voice channel, removing it on leave or the reverse of that, reading TTS messages in voice channels, for those without a mic, creating and managing voice channels, and much more!&#x20;

This is the bot you need to make your server more interactive, and bring your community together!

* [Channel - Role linking](commands/commands/linking-and-unlinking.md)
  * Normal linking - A role(s) can be given to a member when they join a channel, and removed when they leave
  * Reverse Linking - A role(s) can be removed from a member when they join a channel, and added when they leave
  * Great for hiding voice reply channels, or music bot command channels when they aren't needed
* [All channel - Role linking](commands/commands/all-linking.md)
  * A role(s) will be given to a member when they join any voice channel, and removed when they leave
  * Option to add exception channels (members aren't given the 'all' role(s) when they join/leave)
  * Normal & Reverse Linking supported
* [Permanent Role Links](commands/commands/permanent-linking.md)
  * A role(s) will be given to a member when they join the voice channel, and will remain after they leave.
  * Normal & Reverse Linking supported
  * Great for easy user verification
* [Voice Channel Generators](commands/commands/voice-channel-generators.md)
  * When a member joins the generator channel a new voice channel is made just for them, and is deleted when there are no more members in the channel.
  * Generators also come with an interface channel, which contains additional configuration for users' private channels.
  * This is highly configurable, dive in and see what you can make!
* [Voice Channel TTS commands](commands/commands/tts-commands.md)
  * TTS commands are used to make the bot read a message in a voice channel
  * Options for multiple languages.
  * Great for users who have no mic and still want to be heard
* Analytics Commands
  * See insights on what's happening in your voice channels.
  * How much time is being spent in them? How many times do people join? How many commands are being used? and more!
  * See beautiful graphs with per-day data or per-hour visualisations, or prefer to analyse yourself? Download an export of the data as a csv.
* [Voice Admin Commands](commands/commands/voice-admin-commands.md)
  * Used to _(un)_mute/_(un)_deafen all members in a voice channel
* [Audit logging (for voice channels)](commands/commands/audit-logging.md)
  * See when members join, leave or change channels, and the roles that are given/removed by the bot.
