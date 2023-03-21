---
title: "Usables"
linkTitle: "Usables"
type: docs
weight: 1
description: >
  Usables Commands
---

# Table of Contents
- [warp](#net_forthecrown_commands_usables_UseCmdCommand$WarpCommand)
- [kit](#net_forthecrown_commands_usables_UseCmdCommand$KitCommand)
- [area_triggers](#net_forthecrown_commands_usables_TriggerNode)
- [usable_block](#net_forthecrown_commands_usables_UsableBlockNode)
- [usable_entity](#net_forthecrown_commands_usables_UsableEntityNode)
- [interactable](#net_forthecrown_commands_usables_InteractableCommands$CommandInteractable)

# Commands
# /warp <a name="net_forthecrown_commands_usables_UseCmdCommand$WarpCommand"></a>
List all warps or warp to the specified location.  
  
Permission: `ftc.commands.warp`  
## Usages
```yaml
/warp
# Lists all warps

/warp create <name>
# Creates a new warp

/warp <warp>
# Uses a <warp>

/warp <warp> <user>
# Makes a <user> use a <warp>

/warp <warp> remove
# Removes a <warp>

/warp <warp> edit destination
# Sets a <warp>'s destination to where you're standing

/warp <warp> edit destination [world=<world>] [pos=<x,y,z>] [yaw=<number>] [pitch=<pitch>]
# Sets the destination to the given options

/warp <warp> edit tests silent
# Shows if the Usage checks of warp will show fail messages

/warp <warp> edit tests silent <true | false>
# Sets if warp will show fail messages or not

/warp <warp> edit tests
# Lists all tests a warp has

/warp <warp> edit tests clear
# Clears all tests in a warp

/warp <warp> edit tests add <test type> [<test value>]
# Adds a <test type> to a warp
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/warp <warp> edit tests add -first <test type> [<test value>]
# Inserts a <test type> to a warp's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/warp <warp> edit tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a warp at an <index>

/warp <warp> edit tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>
```

# /kit <a name="net_forthecrown_commands_usables_UseCmdCommand$KitCommand"></a>
Obtains the specified kit or views all available kits.  
  
Permission: `ftc.commands.kit`  
## Usages
```yaml
/kit
# Lists all kits

/kit create <name>
# Creates a new kit

/kit <kit>
# Uses a <kit>

/kit <kit> <user>
# Makes a <user> use a <kit>

/kit <kit> remove
# Removes a <kit>

/kit <kit> edit items
# Sets the items of a <kit> to the items in your inventory

/kit <kit> edit items list
# Lists all the items in a <kit>

/kit <kit> edit items add
# Adds the item you're holding to a <kit>

/kit <kit> edit items add <item> <amount: number(1..64)>
# Adds an <item> to a <kit>

/kit <kit> edit items remove <index: number(1..)>
# Removes an item at <index> from a <kit>

/kit <kit> edit tests silent
# Shows if the Usage checks of kit will show fail messages

/kit <kit> edit tests silent <true | false>
# Sets if kit will show fail messages or not

/kit <kit> edit tests
# Lists all tests a kit has

/kit <kit> edit tests clear
# Clears all tests in a kit

/kit <kit> edit tests add <test type> [<test value>]
# Adds a <test type> to a kit
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/kit <kit> edit tests add -first <test type> [<test value>]
# Inserts a <test type> to a kit's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/kit <kit> edit tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a kit at an <index>

/kit <kit> edit tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>
```

# /area_triggers <a name="net_forthecrown_commands_usables_TriggerNode"></a>
An FTC command (default description)  
  
Permission: `ftc.usables`  
Aliases: `usable_triggers`, `triggers`  
## Usages
```yaml
/area_triggers -create <name>
# Creates a trigger from your currently selected WorldEdit
# selection (made with //wand, or with //pos1 and //pos2

/area_triggers -create <name> <pos1: x,y,z> <pos2: x,y,z>
# Creates a trigger from the area between <pos1> and <pos2>

/area_triggers <trigger name> type
# Shows a trigger's type

/area_triggers <trigger name> type <type>
# Sets a trigger's type to <type>

/area_triggers <trigger name> remove
# Removes the triggers

/area_triggers <trigger name> info
# Displays admin information about the triggers

/area_triggers <trigger name> data
# Displays the triggers data

/area_triggers <trigger name> data view [<path: nbt path>]
# Displays triggers data, if [path] is set, shows only
# data at that path

/area_triggers <trigger name> data insert <path: nbt path> <tag>
# Inserts a <tag> into triggers data at a <path>

/area_triggers <trigger name> data merge <tag>
# Merges a <tag> into triggers data

/area_triggers <trigger name> data set <tag>
# Completely overwrites the existing triggers data
# and sets it to <tag>

/area_triggers <trigger name> actions
# Lists all actions a triggers has

/area_triggers <trigger name> actions clear
# Clears all actions in a triggers

/area_triggers <trigger name> actions add <action type> [<action value>]
# Adds a <action type> to a triggers
# <action value> allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/area_triggers <trigger name> actions add -first <action type> [<action value>]
# Inserts a <action type> to a triggers's action list's first place
# [<action value>] allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/area_triggers <trigger name> actions remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a action value from a triggers at an <index>

/area_triggers <trigger name> actions remove -between <start index> <end index>
# Removes all action values between the <start index>
# and <end index>

/area_triggers <trigger name> tests silent
# Shows if the Usage checks of triggers will show fail messages

/area_triggers <trigger name> tests silent <true | false>
# Sets if triggers will show fail messages or not

/area_triggers <trigger name> tests
# Lists all tests a triggers has

/area_triggers <trigger name> tests clear
# Clears all tests in a triggers

/area_triggers <trigger name> tests add <test type> [<test value>]
# Adds a <test type> to a triggers
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/area_triggers <trigger name> tests add -first <test type> [<test value>]
# Inserts a <test type> to a triggers's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/area_triggers <trigger name> tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a triggers at an <index>

/area_triggers <trigger name> tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>
```

# /usable_block <a name="net_forthecrown_commands_usables_UsableBlockNode"></a>
An FTC command (default description)  
  
Permission: `ftc.usables`  
## Usages
```yaml
/usable_block -create <position: x,y,z>
# Creates a new usable

/usable_block <position: x,y,z> remove
# Removes the block

/usable_block <position: x,y,z> info
# Displays admin information about the block

/usable_block <position: x,y,z> data
# Displays the block data

/usable_block <position: x,y,z> data view [<path: nbt path>]
# Displays block data, if [path] is set, shows only
# data at that path

/usable_block <position: x,y,z> data insert <path: nbt path> <tag>
# Inserts a <tag> into block data at a <path>

/usable_block <position: x,y,z> data merge <tag>
# Merges a <tag> into block data

/usable_block <position: x,y,z> data set <tag>
# Completely overwrites the existing block data
# and sets it to <tag>

/usable_block <position: x,y,z> actions
# Lists all actions a block has

/usable_block <position: x,y,z> actions clear
# Clears all actions in a block

/usable_block <position: x,y,z> actions add <action type> [<action value>]
# Adds a <action type> to a block
# <action value> allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/usable_block <position: x,y,z> actions add -first <action type> [<action value>]
# Inserts a <action type> to a block's action list's first place
# [<action value>] allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/usable_block <position: x,y,z> actions remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a action value from a block at an <index>

/usable_block <position: x,y,z> actions remove -between <start index> <end index>
# Removes all action values between the <start index>
# and <end index>

/usable_block <position: x,y,z> tests silent
# Shows if the Usage checks of block will show fail messages

/usable_block <position: x,y,z> tests silent <true | false>
# Sets if block will show fail messages or not

/usable_block <position: x,y,z> tests
# Lists all tests a block has

/usable_block <position: x,y,z> tests clear
# Clears all tests in a block

/usable_block <position: x,y,z> tests add <test type> [<test value>]
# Adds a <test type> to a block
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/usable_block <position: x,y,z> tests add -first <test type> [<test value>]
# Inserts a <test type> to a block's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/usable_block <position: x,y,z> tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a block at an <index>

/usable_block <position: x,y,z> tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>
```

# /usable_entity <a name="net_forthecrown_commands_usables_UsableEntityNode"></a>
An FTC command (default description)  
  
Permission: `ftc.usables`  
## Usages
```yaml
/usable_entity -create <entity: selector>
# Creates a new usable

/usable_entity <entity: selector> remove
# Removes the entity

/usable_entity <entity: selector> info
# Displays admin information about the entity

/usable_entity <entity: selector> data
# Displays the entity data

/usable_entity <entity: selector> data view [<path: nbt path>]
# Displays entity data, if [path] is set, shows only
# data at that path

/usable_entity <entity: selector> data insert <path: nbt path> <tag>
# Inserts a <tag> into entity data at a <path>

/usable_entity <entity: selector> data merge <tag>
# Merges a <tag> into entity data

/usable_entity <entity: selector> data set <tag>
# Completely overwrites the existing entity data
# and sets it to <tag>

/usable_entity <entity: selector> actions
# Lists all actions a entity has

/usable_entity <entity: selector> actions clear
# Clears all actions in a entity

/usable_entity <entity: selector> actions add <action type> [<action value>]
# Adds a <action type> to a entity
# <action value> allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/usable_entity <entity: selector> actions add -first <action type> [<action value>]
# Inserts a <action type> to a entity's action list's first place
# [<action value>] allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/usable_entity <entity: selector> actions remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a action value from a entity at an <index>

/usable_entity <entity: selector> actions remove -between <start index> <end index>
# Removes all action values between the <start index>
# and <end index>

/usable_entity <entity: selector> tests silent
# Shows if the Usage checks of entity will show fail messages

/usable_entity <entity: selector> tests silent <true | false>
# Sets if entity will show fail messages or not

/usable_entity <entity: selector> tests
# Lists all tests a entity has

/usable_entity <entity: selector> tests clear
# Clears all tests in a entity

/usable_entity <entity: selector> tests add <test type> [<test value>]
# Adds a <test type> to a entity
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/usable_entity <entity: selector> tests add -first <test type> [<test value>]
# Inserts a <test type> to a entity's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/usable_entity <entity: selector> tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a entity at an <index>

/usable_entity <entity: selector> tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>
```

# /interactable <a name="net_forthecrown_commands_usables_InteractableCommands$CommandInteractable"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
Aliases: `usable`  
## Usages
```yaml
/interactable triggers -create <name>
# Creates a trigger from your currently selected WorldEdit
# selection (made with //wand, or with //pos1 and //pos2

/interactable triggers -create <name> <pos1: x,y,z> <pos2: x,y,z>
# Creates a trigger from the area between <pos1> and <pos2>

/interactable triggers <trigger name> type
# Shows a trigger's type

/interactable triggers <trigger name> type <type>
# Sets a trigger's type to <type>

/interactable triggers <trigger name> remove
# Removes the triggers

/interactable triggers <trigger name> info
# Displays admin information about the triggers

/interactable triggers <trigger name> data
# Displays the triggers data

/interactable triggers <trigger name> data view [<path: nbt path>]
# Displays triggers data, if [path] is set, shows only
# data at that path

/interactable triggers <trigger name> data insert <path: nbt path> <tag>
# Inserts a <tag> into triggers data at a <path>

/interactable triggers <trigger name> data merge <tag>
# Merges a <tag> into triggers data

/interactable triggers <trigger name> data set <tag>
# Completely overwrites the existing triggers data
# and sets it to <tag>

/interactable triggers <trigger name> actions
# Lists all actions a triggers has

/interactable triggers <trigger name> actions clear
# Clears all actions in a triggers

/interactable triggers <trigger name> actions add <action type> [<action value>]
# Adds a <action type> to a triggers
# <action value> allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/interactable triggers <trigger name> actions add -first <action type> [<action value>]
# Inserts a <action type> to a triggers's action list's first place
# [<action value>] allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/interactable triggers <trigger name> actions remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a action value from a triggers at an <index>

/interactable triggers <trigger name> actions remove -between <start index> <end index>
# Removes all action values between the <start index>
# and <end index>

/interactable triggers <trigger name> tests silent
# Shows if the Usage checks of triggers will show fail messages

/interactable triggers <trigger name> tests silent <true | false>
# Sets if triggers will show fail messages or not

/interactable triggers <trigger name> tests
# Lists all tests a triggers has

/interactable triggers <trigger name> tests clear
# Clears all tests in a triggers

/interactable triggers <trigger name> tests add <test type> [<test value>]
# Adds a <test type> to a triggers
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/interactable triggers <trigger name> tests add -first <test type> [<test value>]
# Inserts a <test type> to a triggers's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/interactable triggers <trigger name> tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a triggers at an <index>

/interactable triggers <trigger name> tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>

/interactable block -create <position: x,y,z>
# Creates a new usable

/interactable block <position: x,y,z> remove
# Removes the block

/interactable block <position: x,y,z> info
# Displays admin information about the block

/interactable block <position: x,y,z> data
# Displays the block data

/interactable block <position: x,y,z> data view [<path: nbt path>]
# Displays block data, if [path] is set, shows only
# data at that path

/interactable block <position: x,y,z> data insert <path: nbt path> <tag>
# Inserts a <tag> into block data at a <path>

/interactable block <position: x,y,z> data merge <tag>
# Merges a <tag> into block data

/interactable block <position: x,y,z> data set <tag>
# Completely overwrites the existing block data
# and sets it to <tag>

/interactable block <position: x,y,z> actions
# Lists all actions a block has

/interactable block <position: x,y,z> actions clear
# Clears all actions in a block

/interactable block <position: x,y,z> actions add <action type> [<action value>]
# Adds a <action type> to a block
# <action value> allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/interactable block <position: x,y,z> actions add -first <action type> [<action value>]
# Inserts a <action type> to a block's action list's first place
# [<action value>] allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/interactable block <position: x,y,z> actions remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a action value from a block at an <index>

/interactable block <position: x,y,z> actions remove -between <start index> <end index>
# Removes all action values between the <start index>
# and <end index>

/interactable block <position: x,y,z> tests silent
# Shows if the Usage checks of block will show fail messages

/interactable block <position: x,y,z> tests silent <true | false>
# Sets if block will show fail messages or not

/interactable block <position: x,y,z> tests
# Lists all tests a block has

/interactable block <position: x,y,z> tests clear
# Clears all tests in a block

/interactable block <position: x,y,z> tests add <test type> [<test value>]
# Adds a <test type> to a block
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/interactable block <position: x,y,z> tests add -first <test type> [<test value>]
# Inserts a <test type> to a block's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/interactable block <position: x,y,z> tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a block at an <index>

/interactable block <position: x,y,z> tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>

/interactable entity -create <entity: selector>
# Creates a new usable

/interactable entity <entity: selector> remove
# Removes the entity

/interactable entity <entity: selector> info
# Displays admin information about the entity

/interactable entity <entity: selector> data
# Displays the entity data

/interactable entity <entity: selector> data view [<path: nbt path>]
# Displays entity data, if [path] is set, shows only
# data at that path

/interactable entity <entity: selector> data insert <path: nbt path> <tag>
# Inserts a <tag> into entity data at a <path>

/interactable entity <entity: selector> data merge <tag>
# Merges a <tag> into entity data

/interactable entity <entity: selector> data set <tag>
# Completely overwrites the existing entity data
# and sets it to <tag>

/interactable entity <entity: selector> actions
# Lists all actions a entity has

/interactable entity <entity: selector> actions clear
# Clears all actions in a entity

/interactable entity <entity: selector> actions add <action type> [<action value>]
# Adds a <action type> to a entity
# <action value> allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/interactable entity <entity: selector> actions add -first <action type> [<action value>]
# Inserts a <action type> to a entity's action list's first place
# [<action value>] allows you to specify data for the <action type>
# to use. The format of data required here, is determined
# by the <action type>

/interactable entity <entity: selector> actions remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a action value from a entity at an <index>

/interactable entity <entity: selector> actions remove -between <start index> <end index>
# Removes all action values between the <start index>
# and <end index>

/interactable entity <entity: selector> tests silent
# Shows if the Usage checks of entity will show fail messages

/interactable entity <entity: selector> tests silent <true | false>
# Sets if entity will show fail messages or not

/interactable entity <entity: selector> tests
# Lists all tests a entity has

/interactable entity <entity: selector> tests clear
# Clears all tests in a entity

/interactable entity <entity: selector> tests add <test type> [<test value>]
# Adds a <test type> to a entity
# <test value> allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/interactable entity <entity: selector> tests add -first <test type> [<test value>]
# Inserts a <test type> to a entity's test list's first place
# [<test value>] allows you to specify data for the <test type>
# to use. The format of data required here, is determined
# by the <test type>

/interactable entity <entity: selector> tests remove <index: number(1..)> [-at <index: number(1..)>]
# Removes a test value from a entity at an <index>

/interactable entity <entity: selector> tests remove -between <start index> <end index>
# Removes all test values between the <start index>
# and <end index>
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Tue Mar 21 15:10:51 EET 2023`  
Plugin version: `1.19.4-1719-SNAPSHOT`  
Total commands: 6