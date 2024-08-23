---
description: >-
  This document provides an overview of the configuration options available in
  the settings.yml
---

# settings.yml

### General Settings

* `language`: This setting determines the language used by the application. It's a string value and the default is `en_US`.
* `proxy-mode`: This is a boolean setting that controls whether the application should run in proxy mode. If set to `true`, the application will run in proxy mode. If set to `false`, it will not.

Here's an example of how these settings might look in the `settings.yml` file:

```yaml
general:
    language: en_US
    proxy-mode: false
```
