---
description: This document provides an overview of the commands and permissions
---

# Commands And Permissions

### Bukkit Commands

#### `/sayanvanish`

* Description: Main command for the SayanVanish plugin.
* Permission: `sayanvanish.commands.use`
* Usage: `/sayanvanish [player] [--state on/off] [-s]`
* Flags:
  * `--state on/off`: Sets the vanish state of the player to either on or off.
  * `-s`: Executes the command silently.

#### `/sayanvanish help`

* Description: Displays the help menu for the SayanVanish plugin.
* Permission: `sayanvanish.commands.help`
* Usage: `/sayanvanish help [query]`

#### `/sayanvanish paste`

* Description: Generates a paste of the current settings and server data.
* Permission: `sayanvanish.commands.paste`
* Usage: `/sayanvanish paste`

#### `/sayanvanish reload`

* Description: Reloads the SayanVanish plugin.
* Permission: `sayanvanish.commands.reload`
* Usage: `/sayanvanish reload`

#### `/sayanvanish level set`

* Description: Sets the vanish level of a player.
* Permission: `sayanvanish.commands.level.set`
* Usage: `/sayanvanish level set <player> <level>`

#### `/sayanvanish level get`

* Description: Gets the vanish level of a player.
* Permission: `sayanvanish.commands.level.get`
* Usage: `/sayanvanish level get <player>`

#### `/sayanvanish forceupdate`

* Description: Will update your plugin jar file and will be applied on next server restart
* Permission: `sayanvanish.commands.forceupdate`
* Usage: `/sayanvanish forceupdate`

### Bukkit Permissions

* `sayanvanish.commands.vanish`: Allows the use of the `/sayanvanish` command.
* `sayanvanish.commands.help`: Allows the use of the `/sayanvanish help` command.
* `sayanvanish.commands.paste`: Allows the use of the `/sayanvanish paste` command.
* `sayanvanish.commands.reload`: Allows the use of the `/sayanvanish reload` command.
* `sayanvanish.commands.level.set`: Allows the use of the `/sayanvanish level set` command.
* `sayanvanish.commands.level.get`: Allows the use of the `/sayanvanish level get` command.
* `sayanvanish.action.vanish.onjoin`: Applies vanish on join
* `sayanvanish.action.vanish.invulnerable`: Keeps invulnerability after unvanish
* `sayanvanish.action.vanish.fly`

### Proxy Commands

#### `/sayanvanishproxy`

* Description: Main command for the SayanVanish plugin on proxies.
* Permission: `sayanvanish.commands.use`
* Usage: `/sayanvanish [player] [--state on/off] [-s]`
* Flags:
  * `--state on/off`: Sets the vanish state of the player to either on or off.
  * `-s`: Executes the command silently.

#### `/sayanvanishproxy forceupdate`

* Description: Will update your plugin jar file and will be applied on next server restart
* Permission: `sayanvanish.commands.forceupdate`
* Usage: `/sayanvanish forceupdate`

### Proxy Permissions

* `sayanvanish.commands.use`: Allows the use of the `/sayanvanishproxy` command.

Please note that these permissions need to be added to your server's permission management system (like LuckPerms) to take effect.
