---
title: "Scripting"
linkTitle: "Scripting"
weight: 2
description: >
  Everything related to using interactables in scripts.
---

{{% pageinfo %}}
Interactables or Usables are blocks/entities/triggers that have special conditions and actions attached to them.
{{% /pageinfo %}}


There are differences in the functions that usables scripts should implement, 
they operate with some commonalities.

Usables scripts will have the following bindings:
- `_holder`: The holder of the action/test, may be a `Kit`, `Warp`, `UsableBlock`, `UsableEntity` or `UsableTrigger`.
- `_entity`: The entity this action/check belongs to, if the action/check is not held by an entity, this will be `undefined`.
- `_block`: The block that this action/check belongs to, if this doesn't belong to a block, this will be `undefined`.
- `_location`: If either `_block` or `_entity` is defined, this will be set to their location.
- `_bounds`: If this action/check belongs to a `UsableTrigger`, this will be set to the trigger's bounds, else, `undefined`

The script systems provides 2 methods to allow for persistent objects. 
  
Use `getDataObject()` to get a native JavaScript object/array/primitive, will 
be null, if the script has no persistent data already saved.
  
Use `setDataObject(object)` to set the persistent data of the script, this must
be a primitive or a native JavaScript object/array that will be saved to JSON.

## Parsing <a name="scripts_parsing"></a>
Script types accept the following input:
`<script name> [<args: string[]>]`, with `<args>` being a comma-separated list 
of argument supplied to the script.
  
For example, a command to add a `run_script` action a script would look like so:
```txt
/usable triggers <name> actions add run_script <script name> [<args>]
```

## Action Scripts <a name="scripts_actions"></a>
Action scripts only need to implement a single method: `onUse(user)`, where 
the `user` is a `net.forthecrown.user.User`;
  
Example of implementation:
```js
function onUse(user) {
  user.sendMessage(Component.text("Hello :D")));
}
```
## Test Scripts <a name="scripts_tests"></a>
The main method a test script needs to implement is `test(user)`. This method 
must return a `true` or `false` value.  
Test scripts can optionally implement 2 more functions, `onTestsPassed(user)` 
and `getFailMessage(user)`;
  
Example of implementation: 
```js
function test(user) {
  return user.getGuild() != null;
}

function onTestsPassed(user) {
  logger.info("User {} passed all tests", user);
}

function getFailMessage(user) {
  return Component.text("You must be in a guild to use this");
}
```