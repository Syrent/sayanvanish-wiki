# FAQ

## "Vanished" Team Warning

Disable the `prevent_push` feature located in the `features` directory, or run the command `/sayanvanish feature disable prevent_push` to turn it off

## Fly turns off after reappearing from vanish

To maintain your flying status when you reappear, you need the `sayanvanish.action.vanish.fly.keep_after_reappear` permission.

## Vanish commands are not recognized

To use the main vanish command, you need the `sayanvanish.commands.use` permission. For other commands, you need the corresponding permission in the format `sayanvanish.commands.<literal1>.<literal2>.<literaln>`.

For example, to use the command `/sayanvanish feature toggleplayer <feature> [player]`, you need the `sayanvanish.commands.feature.toggleplayer` permission.

If you’re using a proxy command (`/sayanvanishproxy`), make sure to quit and rejoin after granting yourself the necessary permissions.

{% content-ref url="commands-and-permissions.md" %}
[commands-and-permissions.md](commands-and-permissions.md)
{% endcontent-ref %}
