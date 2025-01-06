---
description: This feature prevents tab completion for vanished players.
---

# Tab Complete

#### `FeaturePreventTabComplete`

| Parameter          | Description                                                   | Default Value | Possible Values |
| ------------------ | ------------------------------------------------------------- | ------------- | --------------- |
| `checkVanishLevel` | Whether to check vanish levels when filtering tab completions | `false`       | `true`, `false` |

**Behavior:**

* Listens to the `TabCompleteEvent`.
* Filters out tab completion suggestions for vanished players.
* If `checkVanishLevel` is enabled, only filters out suggestions for players with a higher vanish level than the current player.
