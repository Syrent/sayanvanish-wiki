---
description: >-
  This feature checks for updates to the SayanVanish plugin and notifies players
  with the appropriate permissions.
---

# Update

#### `FeatureUpdate`

| Parameter                 | Description                                             | Default Value                         | Possible Values             |
| ------------------------- | ------------------------------------------------------- | ------------------------------------- | --------------------------- |
| `checkEveryXMinutes`      | The interval (in minutes) at which to check for updates | `1440`                                | Any positive integer        |
| `notifyPermission`        | The permission required to receive update notifications | `"sayanvanish.feature.update.notify"` | Any valid permission string |
| `notifyOnJoin`            | Whether to notify players of updates when they join     | `true`                                | `true`, `false`             |
| `notifyForSnapshotBuilds` | Whether to notify players of snapshot builds            | `true`                                | `true`, `false`             |
| `autoUpdateNotification`  | Whether to automatically send update notifications      | `true`                                | `true`, `false`             |

**Behavior:**

* The feature periodically checks for updates to the SayanVanish plugin.
* Players with the specified permission are notified of available updates when they join the server.
* Notifications include links to download the latest release or snapshot builds.
* The feature can also send automatic update requests to players.
