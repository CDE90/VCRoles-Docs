# Voice Linking

{% hint style="danger" %}
These commands are deprecated as they have been replaced by the commands listed [here](linking-and-unlinking.md).
{% endhint %}

Voice linking allows you to automatically give members a role(s) when they join a voice channel, and remove the role(s) once they leave.&#x20;

One great use of Voice Linking is the ability to hide certain channels from members who aren't in the voice channel, for example, a voice reply channel, or a music bot commands channel.

## /voice link

The voice link command is used to create a link between a channel and a role. You can create multiple channel-role links per channel, allowing users to be given a selection of roles when they join a channel.

![](<../../.gitbook/assets/image (13) (1).png>)

{% hint style="warning" %}
The 'VC Roles' role needs to be above the role which you are linking, otherwise, you will not be given the role.
{% endhint %}

## /voice unlink

The voice unlink command is the opposite of the [voice link ](voice-linking.md#vclink)command, removing a channel-role link. Members will not be given roles on joining the channel if you remove the channel-role link.

![](<../../.gitbook/assets/image (30).png>)

## /voice suffix \[add/remove]

This command makes it so that when you join a voice channel, a suffix is added to your username, and removed when you leave the channel.

E.g. your name before joining could be: `Owner | Mr R3spect` and when you join: `Owner | Mr R3sp3ct OS` with OS being the prefix added (in this case meaning online staff)

![](<../../.gitbook/assets/image (29).png>)

![](<../../.gitbook/assets/image (6).png>)
