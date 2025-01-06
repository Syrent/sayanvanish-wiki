---
description: >-
  This feature integrates with the Velocitab plugin to manage vanish states and
  visibility of players.
---

# Velocitab

#### `FeatureHookVelocitab`

| Parameter                       | Description                                                                        | Default Value | Possible Values      |
| ------------------------------- | ---------------------------------------------------------------------------------- | ------------- | -------------------- |
| `checkOnPostServerConnectDelay` | The delay (in milliseconds) before checking vanish state after server post connect | `150`         | Any positive integer |
| `checkOnServerConnectedDelay`   | The delay (in milliseconds) before checking vanish state after server connected    | `150`         | Any positive integer |
| `checkOnPostLoginDelay`         | The delay (in milliseconds) before checking vanish state after post login          | `150`         | Any positive integer |

**Behavior:**

* Registers a vanish integration with the Velocitab plugin.
* Manages vanish states for players using the Velocitab API.
* Provides methods to set, check, and unset vanish states for players.
* Listens to various events (`PostLoginEvent`, `ServerConnectedEvent`, `ServerPostConnectEvent`, `VelocityUserVanishEvent`, `VelocityUserUnVanishEvent`) to manage vanish states accordingly.
