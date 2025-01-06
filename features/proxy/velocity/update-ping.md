---
description: This feature updates the server ping response to exclude vanished players.
---

# Update Ping

#### `FeatureUpdatePing`

**Behavior:**

* Listens to the `ProxyPingEvent`.
* Modifies the server ping response to exclude vanished players from the online player count and sample player list.
