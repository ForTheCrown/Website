---
title: "Usage"
linkTitle: "Usage"
weight: 1
description: >
  Everything related to using interactables.
---

{{% pageinfo %}}
Interactables or Usables are blocks/entities/triggers that have special conditions and actions attached to them.
{{% /pageinfo %}}


  
Usables are made of 2 parts, checks and actions. Checks are run to test if
a player is able to use the object, if all tests are passed, then the actions
will be run.
  
Usable objects also have a `silent` value, this determines if usable objects show
failure messages when a player fails a check.

## Commands <a name="usables_commands"></a>
All usables commands will be prefixed with some arguments, for example:
```txt
/usable entity @e[distance=..2,limit=1] tests remove 0
|----------------- Prefix ------------------|
```
Usages:
```yml
${Prefix}
# Lists all actions/checks

${Prefix} add <type: usage_type> [<input>]
# Adds a check/action of a <type> to the object <input> is optional, 
# depending on the <type> used. For example, 'one_use' check takes no 
# input,  while 'has_permission' check requires a permission name 
# as input.

${Prefix} clear
# Clears all checks/actions on an object

${Prefix} remove <index: number(1..)>
# Removes a check/action at an <index>

${Prefix} remove -between <first index> <last index>
# Removes all actions/checks between the first and second index

${Prefix} remove -with_type <type>
# Removes all actions/checks with the matching <type>
```
See [`/usable` usages](https://github.com/ForTheCrown/FTC/wiki/Commands#interactable-) for more info

## Triggers <a name="usables_triggers"></a>
Triggers are areas that when entered/exited execute the use tests and actions
they have been assigned.
  
To create area triggers, create an area selection with a WorldEdit wand and then
use `/usable triggers -create <name>`.
  
Triggers have a set `type` which determines if actions are ran when a player 
enters or exits or moves while inside the trigger. The type can be changed with
`/usable triggers <trigger name> type <exit|enter|either|move>`.   
  
`exit` and `enter` types are self-explanatory, `either` is run either when a 
player enters or exits the trigger and `move` is run anytime the player moves 
while inside the trigger.

## Blocks <a name="usables_blocks"></a>
Simply a block with usable data attached to it. Note: Blocks must be Tile 
Entities to be used as usables.
  
Usable blocks are accessed with `/usable block <pos: x,y,z>`
  
Blocks share a value with Usable Entities, that is the `cancelVanilla` value,
this determines if vanilla interaction is canceled when using a usable entity,
for example, if a usable chest block is interacted with, then if `cancelVanilla = true`,
the player won't open the chest after the checks and actions have been ran

## Entities <a name="usables_entities"></a>
Simply an entity with usable data attached to it.
  
Usable entities are accessed with `/usable entity <selector>`