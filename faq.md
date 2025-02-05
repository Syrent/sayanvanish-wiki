# FAQ

## "Vanished" Team Warning

Disable the `prevent_push` feature located in the `features` directory, or run the command `/sayanvanish feature disable prevent_push` to turn it off

## Fly turns off after reappearing from vanish

To maintain your flying status when you reappear, you need the `sayanvanish.action.vanish.fly.keep_after_reappear` permission.

## Vanish commands are not recognized

To use the main vanish command, you need the `sayanvanish.commands.use` permission. For other commands, you need the corresponding permission in the format `sayanvanish.commands.<literal1>.<literal2>.<literaln>`.

For example, to use the command `/sayanvanish feature toggleplayer <feature> [player]`, you need the `sayanvanish.commands.feature.toggleplayer` permission.

If you’re using a proxy command (`/sayanvanishproxy`), make sure to quit and rejoin after granting yourself the necessary permissions.

## SayanVanish Doesn't Recognize `*` Permission or Operator Status

There are two possible scenarios:

1. **Proxy Permission**: Some permissions depend on processes managed by the proxy (e.g., Velocity, Bungeecord). To use these permissions, you'll need a plugin like LuckPermsVelocity.
2. **LuckPerms Integration**: If LuckPerms is installed on your server and you're using its permission check inside `hook_luckperms` feature, SayanVanish will use LuckPerms API to handle permissions. To change this behavior, you can disable the `check-permission-via-luckperms` option in `hook_luckperms.yml` within the `features` directory. You can do this using the command `/sayanvanish feature hook_luckperms update checkPermissionViaLuckPerms false`. Alternatively (**Recommended**), you can assign specific permissions using LuckPerms. For instance, if you want to have vanish-on-join permission, you should grant `sayanvanish.action.vanish.onjoin`. If you need to use the vanish feature, assign `sayanvanish.vanish.use` directly.

## I can see myself in TAB

That normal. you and all user that have the same or higher vanish level can see your account in tablist and other places. players without vanish permission or lower vanish levels can't see you.



{% content-ref url="commands-and-permissions.md" %}
[commands-and-permissions.md](commands-and-permissions.md)
{% endcontent-ref %}
