# Voice Generator Interface

When you create a new voice channel generator ([using /voicegenerator](commands/commands/voice-channel-generators.md#voicegenerator)), a text channel will be created alongside the voice channel.

An interface message will get sent to this channel:

![](<.gitbook/assets/image (23).png>)

Reacting to this message with the emojis listed will edit something about your generated VC.

* 🔒 - Locks your voice channel - stops anyone from being able to join your voice channel
* 🔓 - Unlocks your voice channel - allows other members to join your voice channel
* 🚫 - Hides your voice channel - hides your voice channel from the channels list
* 👁 - Unhides your voice channel - your voice channel will be revealed on the channels list
* ⬆ - Increases the user limit of your VC - increases the number of people able to join your voice channel
* ⬇ - Decreases the user limit of your VC - decreases the number of people able to join your voice channel **decreasing the limit to 0, allows an unlimited number of people to join**

****

If you don't want your members to be able to use the generator interface, you can simply delete the text channel, or remove read permissions.
