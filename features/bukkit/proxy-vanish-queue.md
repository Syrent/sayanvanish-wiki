---
description: >-
  This feature manages the visibility of vanished players based on their vanish
  level.
---

# Proxy Vanish Queue

#### `FeatureProxyVanishQueue`

This feature checks a proxy vanish queue at regular intervals and updates the vanish state of players accordingly.

| Parameter    | Description                                           | Default Value | Possible Values         |
| ------------ | ----------------------------------------------------- | ------------- | ----------------------- |
| `checkEvery` | The interval (in ticks) at which the queue is checked | `100`         | Any positive long value |
