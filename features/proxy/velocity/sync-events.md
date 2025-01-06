---
description: >-
  This feature synchronizes vanish events by periodically checking the vanish
  state of users and firing appropriate events.
---

# Sync Events

#### `FeatureSyncEvents`

| Parameter           | Description                                         | Default Value | Possible Values      |
| ------------------- | --------------------------------------------------- | ------------- | -------------------- |
| `checkPeriodMillis` | The period (in milliseconds) to check vanish states | `50`          | Any positive integer |

**Behavior:**

* Periodically checks the vanish state of users.
* Fires `VelocityUserVanishEvent` when a user becomes vanished.
* Fires `VelocityUserUnVanishEvent` when a user becomes unvanished.
