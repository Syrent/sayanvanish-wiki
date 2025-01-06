---
description: >-
  This feature manages the vanish state of players when they join or quit the
  server.
---

# State

{% hint style="danger" %}
This is a **Critical** feature. Do **NOT** disable this feature.
{% endhint %}

#### `FeatureState`

| Parameter               | Description                                                   | Default Value | Possible Values |
| ----------------------- | ------------------------------------------------------------- | ------------- | --------------- |
| `remember`              | Whether to remember the vanish state of players               | `true`        | `true`, `false` |
| `vanishOnJoin`          | Whether to automatically vanish players when they join        | `false`       | `true`, `false` |
| `reappearOnQuit`        | Whether to automatically make players reappear when they quit | `false`       | `true`, `false` |
| `checkPermissionOnQuit` | Whether to check vanish permission when players quit          | `true`        | `true`, `false` |
| `checkPermissionOnJoin` | Whether to check vanish permission when players join          | `true`        | `true`, `false` |

**Behavior:**

* When a player joins, their vanish state is managed based on the configuration and their permissions.
* When a player quits, their vanish state is updated and optionally reset based on the configuration and their permissions.
