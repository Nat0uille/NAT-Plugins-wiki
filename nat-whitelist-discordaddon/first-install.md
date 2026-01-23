---
icon: gears
---

# First Install

1. Put `NAT-Whitelist-XXX.jar` in **/plugins** folder.
2. Reboot the server.

{% stepper %}
{% step %}
### Install the plugin

1. Go to [https://modrinth.com/plugin/nat-whitelist-discordaddon](https://modrinth.com/plugin/nat-whitelist-discordaddon) and get the latest version.
2. Put `NAT-Whitelist-DiscordAddon-XXX.jar` in **/plugins** folder.
3. Reboot the server.
{% endstep %}

{% step %}
### Go into config

You must go to:

```
/plugins/NAT-Whitelist-DiscordAddon/config.yml
```
{% endstep %}

{% step %}
### Add your Discord bot token

Go to [https://discord.com/developers/applications](https://discord.com/developers/applications) and create a new application

After this, go to Bot and reset token

Copy this dans paste to&#x20;

```
discord-bot-token: "YOUR TOKEN HERE"
```
{% endstep %}

{% step %}
### Restart your server

Simply restart `/restart` in your console server
{% endstep %}
{% endstepper %}
