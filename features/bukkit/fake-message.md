---
description: This feature sends fake join and quit messages for vanished players.
---

# Fake Message

#### `FeatureFakeMessage`

| Parameter                      | Description                                        | Default Value                      | Possible Values |
| ------------------------------ | -------------------------------------------------- | ---------------------------------- | --------------- |
| `sendFakeJoinMessage`          | Whether to send a fake join message                | `false`                            | `true`, `false` |
| `sendFakeQuitMessage`          | Whether to send a fake quit message                | `false`                            | `true`, `false` |
| `fakeJoinMessage`              | The fake join message to send                      | `<yellow><player> joined the game` | Any string      |
| `fakeQuitMessage`              | The fake quit message to send                      | `<yellow><player> left the game`   | Any string      |
| `disableJoinMessageIfVanished` | Disable the join message if the player is vanished | `true`                             | `true`, `false` |
| `disableQuitMessageIfVanished` | Disable the quit message if the player is vanished | `true`                             | `true`, `false` |
