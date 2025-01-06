---
description: This feature allows vanished players to interact with containers silently.
---

# Silent Container

#### `FeatureSilentContainer`

| Parameter   | Description                                            | Default Value | Possible Values |
| ----------- | ------------------------------------------------------ | ------------- | --------------- |
| `condition` | Whether the feature is enabled based on server version | `true`        | `true`, `false` |

**Behavior:**

* When a vanished player interacts with a container, their game mode is temporarily switched to spectator mode.
* The player's original game mode and flight status are restored after the interaction.
* Teleportation is restricted while interacting with containers.
