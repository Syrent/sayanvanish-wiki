# Installation

{% hint style="warning" %}
SayanVanish needs an active internet connection to be enabled on your server. Ensure your server is connected to the internet during the initial startup.
{% endhint %}

### Bukkit Installation

1. **Download the Plugin**
   * Download the SayanVanish Bukkit jar file from [Hangar](https://hangar.papermc.io/Syrent/SayanVanish) or [Modrinth](https://modrinth.com/plugin/sayanvanish).
2. **Install the Plugin**
   * Place the downloaded jar file inside the `plugins` folder.
3. **Restart the Server**
   * Restart your Minecraft server to load the plugin.

{% hint style="danger" %}
Do **NOT** copy and paste the SayanVanish directory across multiple servers. The `settings.yml` file contains a unique ID generated during the plugin's first startup. Duplicating this file could lead to synchronization issues.
{% endhint %}

#### Optional Steps

* **Configure Database**
  * Modify the `database.yml` file to change the database type if necessary.
* **Customize Features**
  * Adjust settings in the `features` folder to enable or disable specific features.
* **Setup Permissions**
  * Configure the appropriate permissions for your users.

{% content-ref url="configuration/settings.yml.md" %}
[settings.yml.md](configuration/settings.yml.md)
{% endcontent-ref %}

{% content-ref url="configuration/database.yml.md" %}
[database.yml.md](configuration/database.yml.md)
{% endcontent-ref %}

{% content-ref url="configuration/less-than-feature-greater-than.yml.md" %}
[less-than-feature-greater-than.yml.md](configuration/less-than-feature-greater-than.yml.md)
{% endcontent-ref %}

### Proxy (Velocity/Bungeecord) Installation

{% hint style="info" %}
Using proxy modules to sync data between servers is not necessary. These modules enable the `%sayanvanish_online_tota%` and `%sayanvanish_online_<server>%` placeholders and allow API calls from Velocity to backend servers.
{% endhint %}

1. **Download the Plugin**
   * Download the SayanVanish Velocity/Bungeecord jar file from [Hangar](https://hangar.papermc.io/Syrent/SayanVanish) or [Modrinth](https://modrinth.com/plugin/sayanvanish).
2. **Install the Plugin**
   * Place the downloaded jar file in your `plugins` directory.
3. **Restart the Proxy**
   * Restart your proxy server to load the plugin.
4. **Configure Database on Proxy**
   * Navigate to the `SayanVanish` folder on your proxy server and change the database method to MySQL or Redis.
5. **Configure Database on Backend Servers**
   * On each of your backend servers, change the database method to MySQL or Redis.
6. **Enable Proxy Mode**
   * Set `proxy-mode` to `true` in the `settings.yml` file on your backend servers.
7. **Restart Servers**
   * Restart both your proxy and backend servers to apply the changes.
