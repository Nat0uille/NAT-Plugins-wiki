---
icon: earth-africa
---

# Add language

You can add a custom language to the plugin by creating your own translation file. Follow the steps below.

### 1️⃣ Create the language file

Inside the plugin’s `lang/` folder, create a new file:

```
fr-fr.yml
```

You can replace `fr-fr` with any language code you want to use.

### 2️⃣ Copy the translation keys

Open one of the default language files (e.g. `en-us.yml`) and copy **all keys** into your new file.\
Only translate the values.

{% hint style="warning" %}
**Do not change the keys**, only the text after `:`
{% endhint %}

### 3️⃣ Set the language in `config.yml`

In the plugin configuration file, update the `lang` field:

```yaml
lang: fr-fr
```

👉 Use **only the file name without `.yml`**.

### 4️⃣ Restart or reload the plugin

Apply the changes by restarting the server or using the reload command.

```yaml
/nat-whitelist reload
```
