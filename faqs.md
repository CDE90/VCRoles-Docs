# FAQs

Here is a selection of VC Roles FAQs, if you feel like any are missing, let us know in our support server, or make a pull request on github.



### **What is the bot's prefix?**&#x20;

The bot's prefix is `/`

****

### **Why did you switch to slash commands?**&#x20;

We switched to slash commands, as recommended by discord (and since we no longer have access to message content) - you can read more here: ([https://support-dev.discord.com/hc/en-us/articles/4404772028055-Message-Content-Privileged-Intent-for-Verified-Bots](https://support-dev.discord.com/hc/en-us/articles/4404772028055-Message-Content-Privileged-Intent-for-Verified-Bots) [https://support.discord.com/hc/en-us/articles/4410940809111](https://support.discord.com/hc/en-us/articles/4410940809111))



### **What is the bot's website?**&#x20;

The bot's website has moved recently to: [https://www.vcroles.com/](https://www.vcroles.com)





### **The bot's slash commands aren't showing**&#x20;

* If you have just invited the bot to your server, it may take up to a minute for slash commands to show, and you may also need to reload your client. Sadly there is nothing we can do about this, as it is a limitation on discord's end.&#x20;
* If the bot has been in your server for a while (last time you used it, slash commands weren't being used) you may need to re-invite the bot with new permissions using this link: [https://discord.com/api/oauth2/authorize?client\_id=775025797034541107\&permissions=300944400\&scope=bot%20applications.commands](https://discord.com/api/oauth2/authorize?client\_id=775025797034541107\&permissions=300944400\&scope=bot%20applications.commands)&#x20;



### **The bot isn't responding / `Application did not respond` error**

This may be because the bot is offline - this happens occasionally, but we will always do our best to limit downtime.



### **The bot isn't giving me roles**&#x20;

This is likely because the bot doesn't have permissions to give you the role. Make sure the bot has `Manage Roles` permission, and the _VC Roles_ role is above the role that you want the bot to add (in the role list)



### **The channel I want to link isn't showing up in my command**&#x20;

This is likely because the bot doesn't have permissions to see the channel which you are trying to link. To fix this, please make sure that the bot has `View Channel` permissions for the channel you want to link, then try again.



### **The bot is showing as offline**&#x20;

If the bot is offline in the members list, this could be for a few reasons:&#x20;

* We are performing maintenance on either the bot, the database, or the machine the bot is hosted on. This will be announced in our support server.&#x20;
* The bot has gone offline for another reason - while we do our best to keep the bot online, it does occasionally go offline. If this happens, we will get a notification, and we will try to fix the problem as soon as possible.



### **When I try to use TTS it says **_**TTS not enabled**_&#x20;

This is likely because you haven't enabled TTS in your server, to do this, use the command `/ttssetup`. More info can be found on our website here: [https://www.vcroles.com/commands/commands/tts-commands#ttssetup](https://www.vcroles.com/commands/commands/tts-commands#ttssetup)