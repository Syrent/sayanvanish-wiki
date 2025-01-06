---
description: This feature applies potion effects to vanished players.
---

# Effect

#### `FeatureEffect`

| Parameter | Description                                         | Default Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| --------- | --------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `effects` | List of potion effects to apply to vanished players | <p></p><pre><code>effects:
-   use-packet: true
    keep-after-appear: false
    type: NIGHT_VISION
    duration: 2147483647
    amplifier: 0
    ambient: false
    particles: false
-   use-packet: false
    keep-after-appear: false
    type: WATER_BREATHING
    duration: 2147483647
    amplifier: 0
    ambient: false
    particles: false
-   use-packet: false
    keep-after-appear: false
    type: FIRE_RESISTANCE
    duration: 2147483647
    amplifier: 0
    ambient: false
    particles: false
</code></pre> |
