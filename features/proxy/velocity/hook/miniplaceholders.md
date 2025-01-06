---
description: >-
  This feature integrates with the MiniPlaceholders plugin to provide
  vanish-related placeholders.
---

# MiniPlaceholders

#### `FeatureHookMiniPlaceholders`

| Parameter | Description                         | Default Value        | Possible Values       |
| --------- | ----------------------------------- | -------------------- | --------------------- |
| `plugin`  | The name of the plugin to hook into | `"miniplaceholders"` | Any valid plugin name |

**Behavior:**

* Registers a placeholder provider with the MiniPlaceholders plugin.
* Provides placeholders for vanished state, vanish level, and online player counts excluding vanished players.
