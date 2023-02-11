---
title: "Task Scheduling"
linkTitle: "Task Scheduling"
weight: 3
description: >
  Everything related to task scheduling.
---

FTC's scripting abstractions allow for the scheduling of delayed and repeating tasks.  
  
All tasks that can be scheduled will be executed on the main thread.

## Examples
All intervals passed to the scheduler are measured in ticks, not milliseconds

### Scheduling a delayed task
```js
scheduler.runLater(10 /* Delay in ticks */, task => {
  // Perform some action
});
```
### Scheduling a repeating task
```js
scheduler.runTimer(10 /* Initial Delay */, 10 /* Repeating delay*/, task => {
  
});
```
### Scheduling a task that only runs n number of times
```js
const MAX_RUNS = 20;
var runCount = 0;

scheduler.runTimer(10, 10, task => {
  // Increment run count tracker
  ++runCount;
  
  // If run count surpasses max runs, stop execution
  if (runCount >= MAX_RUNS) {
    task.cancel();
  }
});
```
## TaskWrapper class
The task class passed to scheduler methods is not the bukkit `BukkitTask` class, rather it's a wrapper with some additional functionality.  
If you need to access the actual bukkit task you can do so with `task.getTask()`.  
It is also heavily reccommended you use `task.cancel()` for cancelling tasks instead of `task.getTask().cancel()`

## Extra
- [`ScriptTasks`](../tree/main/src/main/java/net/forthecrown/core/script2/ScriptTasks.java)