---
description: >-
  This feature checks for updates and notifies users about new versions of the
  plugin.
---

# Update

#### `FeatureUpdate`

| Parameter                   | Description                                                 | Default Value                                | Possible Values             |
| --------------------------- | ----------------------------------------------------------- | -------------------------------------------- | --------------------------- |
| `checkEveryXMinutes`        | The interval (in minutes) to check for updates              | `1440`                                       | Any positive integer        |
| `notifyBypassPermission`    | The permission that exempts users from update notifications | `"sayanvanish.feature.update.notify.exempt"` | Any valid permission string |
| `notifyOnJoin`              | Whether to notify users about updates when they join        | `true`                                       | `true`, `false`             |
| `notifyForSnapshotBuilds`   | Whether to notify users about snapshot builds               | `true`                                       | `true`, `false`             |
| `autoUpdateNotification`    | Whether to automatically send update notifications          | `true`                                       | `true`, `false`             |
| `updateNotificationContent` | The content of the update notification message              | List of strings                              | Any list of strings         |
| `updateRequestContent`      | The content of the update request message                   | List of strings                              | Any list of strings         |

**Behavior:**

* Periodically checks for updates using `HangarUtils`.
* Notifies users about new releases and snapshots.
* Sends update notifications and requests to users based on configuration.
* Provides methods to download and install updates.
