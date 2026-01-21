---
description: How install the plugin & default config
icon: gears
---

# First Install

{% stepper %}
{% step %}
### Install the plugin

1. Go to [modrinth.com/plugin/nat-whitelist](https://modrinth.com/plugin/nat-whitelist) and get the latest version.
2. Put `NAT-Whitelist-XXX.jar` in **/plugins** folder.
3. Reboot the server.


{% endstep %}

{% step %}
### Go into config

You must go to:

```
/plugins/NAT-Whitelist/config.yml
```
{% endstep %}

{% step %}
### Chose where to save data

**There are two choices for database types:**

| Type      | Description                                                                                                                                |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **H2**    | Local storage in a `database.db` file inside the plugin folder. Recommended for small configurations or servers with no external database. |
| **MySQL** | Storage on an external database. Ideal for multi-server servers or if you want to back up your data separately.                            |
| MariaDB   | Storage on an external database. Ideal for multi-server servers or if you want to back up your data separately.                            |

```yml
database:
  type: H2
  host: localhost
  port: 3306
  database: nat_whitelist
  username: ''
  password: ''
```
{% endstep %}

{% step %}
## Select a language

You have a choice of languages\
If you want a customized language, check :

{% content-ref url="add-language.md" %}
[add-language.md](add-language.md)
{% endcontent-ref %}

```yml
# Language of the plugin (en-us / fr-fr)
lang: en-us
```
{% endstep %}

{% step %}
### Restart the server

Simply restart `/restart` in your console server
{% endstep %}
{% endstepper %}
