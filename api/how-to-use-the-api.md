# How to Use the API

SayanVanish contains an extensive API to perform all necessary actions. To start, add the SayanVanish dependency to your build tool of choice, such as Maven or Gradle.

#### Adding the Repository

**In Maven**

```xml
<repository>
  <id>repo-sayandevelopment</id>
  <name>SayanDevelopment Repository</name>
  <url>https://repo.sayandev.org/snapshots</url>
</repository>
```

**In Gradle**

* **Groovy**

```groovy
maven {
    url "https://repo.sayandev.org/snapshots"
}
```

* **Kotlin**

```kotlin
maven {
    url = uri("https://repo.sayandev.org/snapshots")
}
```

#### Adding the Dependency

You can use different platform-specific dependencies or the main platform-independent API.

**Main API Dependency**

The dependency artifact for the main API is `sayanvanish-api`.

**Platform-Specific Dependencies**

For platform-specific dependencies, the artifact ID follows the format `sayanvanish-<platform>`. Examples include `sayanvanish-bukkit` and `sayanvanish-proxy-velocity`.

**In Maven**

```xml
<dependency>
  <groupId>org.sayandev</groupId>
  <artifactId>sayanvanish-bukkit</artifactId>
  <version>[get version from github]</version>
</dependency>
```

**In Gradle**

* **Groovy**

```groovy
implementation "org.sayandev:sayanvanish-bukkit:[get version from github]"
```

* **Kotlin**

```kotlin
implementation("org.sayandev:sayanvanish-bukkit:[get version from github]")
```

#### Accessing the API

You can access the SayanVanish API like this:

```java
SayanVanishAPI.getInstance();
```

Or you can use a platform-specific user type like this:

```java
SayanVanishAPI<BukkitUser>.getInstance();
```

Or like this:

```java
SayanVanishBukkitAPI.getInstance();
```

From this class, you can access and modify everything. For example, to add a new user:

```java
SayanVanishAPI.getInstance().addUser(User);
```

Or to access the database directly:

```java
SayanVanishAPI.getInstance().getDatabase();
```

#### Events

There are two Bukkit-specific events you can use: `BukkitUserVanishEvent` and `BukkitUserUnVanishEvent`. Both events contain the user and vanish options.

***

For further details and advanced configurations, please refer to the subsequent sections.
