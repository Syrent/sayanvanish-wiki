---
description: This feature allows vanished players to toggle their game mode by sneaking.
---

# Sneak Toggle GameMode

#### `FeatureSneakToggleGameMode`

| Parameter      | Description                                             | Default Value | Possible Values                                  |
| -------------- | ------------------------------------------------------- | ------------- | ------------------------------------------------ |
| `fallbackMode` | The game mode to switch to if no previous mode is found | `SURVIVAL`    | `SURVIVAL`, `CREATIVE`, `ADVENTURE`, `SPECTATOR` |

**Behavior:**

* When a vanished player sneaks, their game mode toggles between their current mode and spectator mode.
* The player's original game mode is restored when they stop sneaking.
* The feature ensures that the player's flight status is preserved during the toggle.
