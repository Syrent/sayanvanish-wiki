---
description: >-
  This feature integrates with the AdvancedServerList plugin to provide
  vanish-related placeholders.
---

# AdvancedServerList

#### `FeatureHookAdvancedServerList`

| Parameter | Description                         | Default Value          | Possible Values       |
| --------- | ----------------------------------- | ---------------------- | --------------------- |
| `plugin`  | The name of the plugin to hook into | `"advancedserverlist"` | Any valid plugin name |

**Behavior:**

* Registers a placeholder provider with the AdvancedServerList plugin.
* Provides placeholders for vanished state, vanish level, and online player counts excluding vanished players.
