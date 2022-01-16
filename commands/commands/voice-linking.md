# Voice Linking

Voice linking allows you to automatically give members a role(s) when they join a voice channel, and remove the role(s) once they leave.&#x20;

One great use of Voice Linking is the ability to hide certain channels from members who aren't in the voice channel, for example, a voice reply channel, or a music bot commands channel.

## /vclink

The vclink command is used to create a link between a channel and a role. You can create multiple channel-role links per channel, allowing users to be given a selection of roles when they join a channel.

![vclink command](<../../.gitbook/assets/image (14).png>)

{% hint style="warning" %}
The 'VC Roles' role needs to be above the role which you are linking, otherwise, you will not be given the role.
{% endhint %}

## /vcunlink

The vcunlink command is the opposite of the [vclink](voice-linking.md#vclink) command, removing a channel-role link. Members will not be given roles on joining the channel if you remove the channel-role link.

![vcunlink command](<../../.gitbook/assets/image (15).png>)
