---
description: >-
  This feature integrates with the EnhancedVelocity plugin to manage vanish
  states.
---

# EnhancedVelocity

#### `FeatureHookEnhancedVelocity`

| Parameter | Description                         | Default Value        | Possible Values       |
| --------- | ----------------------------------- | -------------------- | --------------------- |
| `plugin`  | The name of the plugin to hook into | `"enhancedvelocity"` | Any valid plugin name |

**Behavior:**

* Registers a vanish hook with the EnhancedVelocity plugin.
* Manages vanish states for players using the EnhancedVelocity API.
* Provides methods to set, check, and unset vanish states for players.
