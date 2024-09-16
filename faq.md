# FAQ

## "Vanished" Team Warning

Disable the `prevent_push` feature located in the `features` directory, or run the command `/sayanvanish feature disable prevent_push` to turn it off

## Fly turns off after reappearing from vanish

To maintain your flying status when you reappear, you need the `sayanvanish.action.vanish.fly.keep_after_reappear` permission.

## Vanish commands are not recognized

To use the main vanish command, you need the `sayanvanish.commands.use` permission. For other commands, you need the corresponding permission in the format `sayanvanish.commands.<literal1>.<literal2>.<literaln>`.

For example, to use the command `/sayanvanish feature toggleplayer <feature> [player]`, you need the `sayanvanish.commands.feature.toggleplayer` permission.

If you’re using a proxy command (`/sayanvanishproxy`), make sure to quit and rejoin after granting yourself the necessary permissions.

### SayanVanish Doesn't Recognize `*` Permission or Operator Status

There are two possible scenarios:

1. **Proxy Permission**: Some permissions depend on processes managed by the proxy (e.g., Velocity, Bungeecord). To use these permissions, you'll need a plugin like LuckPermsVelocity.
2. **LuckPerms Integration**: If LuckPerms is installed on your server, SayanVanish will use its API to handle permissions. This helps prevent issues, such as the `sayanvanish.action.vanish.onjoin` permission being automatically granted if you're an operator or have `*` permissions. To change this behavior, you can disable the `check-permission-via-luckperms` option in `hook_luckperms.yml` within the `features` directory. You can do this using the command `/sayanvanish feature hook_luckperms update checkPermissionViaLuckPerms false`. Alternatively (**Recommended**), you can assign specific permissions using LuckPerms. For instance, if you want to have vanish-on-join permission, you should grant `sayanvanish.action.vanish.onjoin`. If you need to use the vanish feature, assign `sayanvanish.vanish.use` directly.

### How can I stop being vanished on join?

The permission that controls vanishing on join is `sayanvanish.action.vanish.onjoin`. If you have operator access or `*` permission, this permission is automatically granted to you, which can lead to unwanted behavior. Installing LuckPerms will resolve this issue since the plugin will use its permission checks to prevent it. However, if you prefer to disable this permission manually on any server, you can use any permission plugin to set this permission to false. For example, with LuckPerms, you can use the command: `/luckperms user <user> permission set sayanvanish.action.vanish.onjoin false`



{% content-ref url="commands-and-permissions.md" %}
[commands-and-permissions.md](commands-and-permissions.md)
{% endcontent-ref %}
