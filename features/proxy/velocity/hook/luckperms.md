---
description: >-
  This feature integrates with the LuckPerms plugin to manage vanish states and
  permissions.
---

# LuckPerms

#### `FeatureLuckPermsHook`

| Parameter                     | Description                                     | Default Value | Possible Values |
| ----------------------------- | ----------------------------------------------- | ------------- | --------------- |
| `registerCustomContext`       | Whether to register a custom context calculator | `true`        | `true`, `false` |
| `checkPermissionViaLuckPerms` | Whether to check permissions via LuckPerms      | `true`        | `true`, `false` |

**Behavior:**

* Registers a custom context calculator with LuckPerms if `registerCustomContext` is enabled.
* Provides methods to check permissions and retrieve permissions for a player using LuckPerms.
* Falls back to default permission check if the feature is not active.
