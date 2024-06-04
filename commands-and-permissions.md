---
description: This document provides an overview of the commands and permissions
---

# Commands And Permissions

### Commands

#### `/sayanvanish`

* Description: Main command for the SayanVanish plugin.
* Permission: `sayanvanish.commands.vanish`
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

### Permissions

* `sayanvanish.commands.vanish`: Allows the use of the `/sayanvanish` command.
* `sayanvanish.commands.help`: Allows the use of the `/sayanvanish help` command.
* `sayanvanish.commands.paste`: Allows the use of the `/sayanvanish paste` command.
* `sayanvanish.commands.reload`: Allows the use of the `/sayanvanish reload` command.
* `sayanvanish.commands.level.set`: Allows the use of the `/sayanvanish level set` command.
* `sayanvanish.commands.level.get`: Allows the use of the `/sayanvanish level get` command.
* `sayanvanish.action.vanish.onjoin`: Applies vanish on join
* `sayanvanish.action.vanish.invulnerable`: Keeps invulnerability after unvanish
* `sayanvanish.action.vanish.fly`



Please note that these permissions need to be added to your server's permission management system (like LuckPerms) to take effect.
