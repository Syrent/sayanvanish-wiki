# \<feature>.yml

In the SayanVanish, features are controlled by individual YAML configuration files. These files allow you to enable, disable, and configure the behavior of each feature. Here's a general guide on how to use and modify them.

### General Structure

Each feature file has a similar structure. Here's a breakdown:

* `id`: This is the unique identifier for the feature. It's a string value and should not be changed.
* `enabled`: This is a boolean setting that controls whether the feature is enabled or not. If set to `true`, the feature will be active. If set to `false`, it will be inactive.

Depending on the feature, there may be additional settings that control the behavior of the feature.

### Example: `level.yml`

```yaml
see-as-spectator: true
id: level
enabled: true
category: DEFAULT
```

In this example, the `level` feature has an additional setting `see-as-spectator`. This is a boolean setting that controls whether users should see other vanished users as a spectator or normal players in tab.

### Example: `effect.yml`

```yaml
effects:
-   use-packet: true
    type: NIGHT_VISION
    duration: 2147483647
    amplifier: 1
    ambient: false
    particles: false
-   use-packet: false
    type: WATER_BREATHING
    duration: 2147483647
    amplifier: 1
    ambient: false
    particles: false
-   use-packet: false
    type: FIRE_RESISTANCE
    duration: 2147483647
    amplifier: 1
    ambient: false
    particles: false
id: effect
enabled: true
category: DEFAULT
```

In this example, the `effect` feature has an additional setting `effects`. This is a list of effects that will be applied. Each effect has the following settings:

* `use-packet`: This is a boolean setting that controls whether to use a packet to apply the effect.
* `type`: This is the type of the effect. It's a string value and can be any valid potion effect type.
* `duration`: This is the duration of the effect in ticks. 20 ticks = 1 second.
* `amplifier`: This is the amplifier of the effect. It's an integer value and determines the level of the effect.
* `ambient`: This is a boolean setting that controls whether the effect is ambient.
* `particles`: This is a boolean setting that controls whether the effect has particles.

### Modifying Features

To modify a feature, simply open the corresponding YAML file and change the settings as needed. Make sure to save the file and restart/reload SayanVanish for the changes to take effect.
