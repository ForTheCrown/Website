---
title: "Listening to Events"
linkTitle: "Event Listeners"
weight: 4
description: >
  Everything related to events listeners in scripts.
---


{{% pageinfo %}}
Scripts can register event listeners by using the in-built `events` object.
{{% /pageinfo %}}

## Examples
The following are various examples of how the events object can be used

### Simple event registration
```js
// Declare the Java type
import "@bukkit.event.player.PlayerJoinEvent"

// Register a function to list to the given event
events.register(PlayerJoinEvent, onPlayerJoin);

// Function called when event is triggered
function onPlayerJoin(event) {
  logger.info("Player {} joined the server!", event.getPlayer());
}
```
### Prioritized listener registration
Please see [The Bukkit Wiki](https://bukkit.fandom.com/wiki/Event_API_Reference#:~:text=false-,Event%20Priorities,-There%20are%20six) for information about EventPriority.

```js
import * as EventPrio from "@bukkit.event.EventPriority"

// Register a function to list to the given event with the LOWEST
// priority
events.register(PlayerJoinEvent, onPlayerJoin, EventPrio.LOWEST);
```
### Ignoring cancelled events
This section is very similar to the past one, with simply one extra parameter
```js
// The final parameter states whether events that have been cancelled by
// other listeners that were executed before this listener, should be ignored.
// If true, cancelled events won't call the given function, if false, they will
events.register(PlayerJoinEvent, onPlayerJoin, EventPrio.LOWEST, true);
```
