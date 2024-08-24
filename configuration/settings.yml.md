---
description: >-
  This guide provides detailed explanations for the settings.yml file used to
  configure the SayanVanish plugin. Each setting is outlined below to help you
  understand and customize your server's behavior
---

# settings.yml

#### General Settings

The `general` section contains key configurations for the plugin's operation on your server.

**`server-id`**

{% hint style="danger" %}
Do **NOT** copy and paste the SayanVanish directory across multiple servers. The `server-id` is generated during the plugin's first startup. Duplicating this file could lead to synchronization issues.
{% endhint %}

* **Description**: A unique identifier for your server.
* **Purpose**: This ID is used internally to distinguish your server, specifically in multi-server setups.

**`language`**

{% hint style="info" %}
By default, SayanVanish only includes the `en_US` language. However, you can create and add your own custom languages.
{% endhint %}

* **Description**: The language setting for the plugin.
* **Default Value**: `en_US`
* **Options**: Set this to any valid language file name (without `.yml` extension) from `languages` directory
* **Example**: `fr_FR` for French or `de_DE` for German.

**`proxy-mode`**

{% hint style="info" %}
Enable this option if you're using SayanVanish on a proxy server (such as Bungeecord or Velocity).
{% endhint %}

* **Description**: Toggles proxy mode on or off.
* **Default Value**: `false`
* **Options**:
  * `true`: Enable proxy mode, typically used when running the plugin behind a proxy server.
  * `false`: Disable proxy mode.

**`cache-update-period-ticks`**

* **Description**: The interval, in ticks, at which the plugin updates its cache.
* **Default Value**: `20`
* **Purpose**: Adjust this value to change how frequently the cache is refreshed. Lower values mean more frequent updates.

**`basic-cache-update-period-ticks`**

{% hint style="info" %}
The basic cache is a list of all users across your network and is used to generate custom placeholders and player lists in various locations.
{% endhint %}

* **Description**: The interval, in ticks, for basic cache updates.
* **Default Value**: `20`
* **Purpose**: Similar to `cache-update-period-ticks`, but for basic cache operations.

#### Command Settings

The `command` section allows you to customize the primary command

**`name`**

* **Description**: The main command name for the plugin.
* **Default Value**: `sayanvanish`

**`aliases`**

* **Description**: Alternate names that can be used in place of the main command.
* **Default Values**:
  * `v`
  * `vanish`
  * `sv`
* **Purpose**: These aliases provide flexibility, allowing players to use shorter or more convenient commands.

***

By adjusting these settings in the `settings.yml` file, you can fine-tune how SayanVanish operates on your server. Be sure to restart your server after making any changes to apply them.
