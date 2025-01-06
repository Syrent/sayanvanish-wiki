---
description: >-
  This feature manages the visibility of vanished players based on their vanish
  level.
---

# Level

{% hint style="danger" %}
This is a **Critical** feature. Do **NOT** disable this feature.
{% endhint %}

#### `FeatureLevel`

| Parameter        | Description                                   | Default Value | Possible Values          |
| ---------------- | --------------------------------------------- | ------------- | ------------------------ |
| `seeAsSpectator` | Whether to see vanished players as spectators | `true`        | `true`, `false`          |
| `levelMethod`    | The method used to determine vanish levels    | `PERMISSION`  | `PERMISSION`, `DATABASE` |

**Enum `LevelMethod` values:**

* `PERMISSION`: Use permissions to determine vanish levels.
* `DATABASE`: Use a database to determine vanish levels.
