# Events

In the SayanVanish plugin, there are two main events that you can listen to: `BukkitUserVanishEvent` and `BukkitUserUnVanishEvent`. These events are triggered when a user vanishes or unvanishes respectively.

### BukkitUserVanishEvent

This event is triggered when a user vanishes. You can listen to this event to perform actions when a user vanishes.

#### Example Usage

```java
import org.bukkit.event.EventHandler;
import org.bukkit.event.Listener;
import org.sayandev.sayanvanish.bukkit.api.event.BukkitUserVanishEvent;

public class MyPluginListener implements Listener {

    @EventHandler
    public void onUserVanish(BukkitUserVanishEvent event) {
        // Your code here
        System.out.println(event.getUser().getUsername() + " has vanished!");
    }
}
```

### BukkitUserUnVanishEvent

This event is triggered when a user unvanishes. You can listen to this event to perform actions when a user unvanishes.

#### Example Usage

```java
import org.bukkit.event.EventHandler;
import org.bukkit.event.Listener;
import org.sayandev.sayanvanish.bukkit.api.event.BukkitUserUnVanishEvent;

public class MyPluginListener implements Listener {

    @EventHandler
    public void onUserUnVanish(BukkitUserUnVanishEvent event) {
        // Your code here
        System.out.println(event.getUser().getUsername() + " has unvanished!");
    }
}
```

In both examples, `MyPluginListener` is a class that implements the `Listener` interface. The `onUserVanish` and `onUserUnVanish` methods are marked with the `@EventHandler` annotation to indicate that they are event handlers. When a `BukkitUserVanishEvent` or `BukkitUserUnVanishEvent` is triggered, the corresponding method will be called.
