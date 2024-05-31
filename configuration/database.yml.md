---
description: >-
  This document provides an overview of the configuration options available in
  the database.yml
---

# database.yml

### Database Settings

* `method`: This setting determines the database method used by the application. It's a string value and can be either `SQL` or `SQLite`.
* `sql`: This is a nested setting that contains the configuration for the SQL database. It includes the following sub-settings:
  * `method`: The specific SQL method to use. It can be `MYSQL` or `POSTGRESQL`.
  * `host`: The host address of the SQL server.
  * `port`: The port number of the SQL server.
  * `database`: The name of the database to connect to.
  * `username`: The username for the SQL server.
  * `password`: The password for the SQL server.
  * `pool-properties`: These are properties for the connection pool, including `maximum-pool-size`, `minimum-idle`, `maximum-lifetime`, `keepalive-time`, `connection-timeout`, and `use-ssl`.
  * `table-prefix`: The prefix to use for table names in the database.
* `redis`: This is a nested setting that contains the configuration for the Redis database. It includes the following sub-settings:
  * `type`: The type of Redis setup. It can only be `STANDALONE`.&#x20;
  * `standalone`: This is a nested setting that contains the configuration for a standalone Redis setup. It includes `host`, `port`, `user`, `password`, and `ssl`.
  * `cluster`: This is a nested setting that contains the configuration for a Redis cluster setup. It includes `nodes` (a list of node addresses), `user`, `password`, and `ssl`.
* `use-cache-when-available`: This is a boolean setting that controls whether the application should use cache when it's available.

Here's an example of how these settings might look in the `database.yml` file:

```yaml
method: SQL
sql:
    method: MYSQL
    host: localhost
    port: 3306
    database: sayanvanish
    username: root
    password: admin
    pool-properties:
        maximum-pool-size: 10
        minimum-idle: 10
        maximum-lifetime: 1800000
        keepalive-time: 0
        connection-timeout: 5000
        use-ssl: false
    table-prefix: sayanvanish_
redis:
    type: STANDALONE
    standalone:
        host: localhost
        port: 6379
        user: ''
        password: ''
        ssl: false
use-cache-when-available: true
```

Please note that these settings can be changed according to your requirements. Make sure to restart the application after making any changes for them to take effect.

**Important**: If you are going to use SQLite as your database method, please note that the proxy mode does not work.
