---
title: "Admin"
linkTitle: "Admin"
type: docs
weight: 1
description: >
  Admin Commands
---

# Table of Contents
- [/adventure](#commands_admin_CommandSpecificGameMode)
- [/broadcast](#commands_admin_CommandBroadcast)
- [/cooldown](#commands_admin_CommandCooldown)
- [/creative](#commands_admin_CommandSpecificGameMode)
- [/dungeons](#commands_admin_CommandDungeons)
- [/endopener](#commands_admin_CommandEndOpener)
- [/ftcreload](#commands_admin_SaveReloadCommands)
- [/ftcsave](#commands_admin_SaveReloadCommands)
- [/ftcstruct](#commands_admin_CommandFtcStruct)
- [/ftcversion](#commands_admin_CommandFtcVersion)
- [/getoffset](#commands_admin_CommandGetOffset)
- [/getpos](#commands_admin_CommandGetPos)
- [/gift](#commands_admin_CommandGift)
- [/gm](#commands_admin_CommandGameMode)
- [/hologram](#commands_admin_CommandHologram)
- [/illegalworlds](#commands_admin_CommandIllegalWorlds)
- [/invstore](#commands_admin_CommandInvStore)
- [/joininfo](#commands_admin_CommandJoinInfo)
- [/launch](#commands_admin_CommandLaunch)
- [/makeaward](#commands_admin_CommandMakeAward)
- [/memory](#commands_admin_CommandMemory)
- [/npc](#commands_admin_CommandNPC)
- [/playertime](#commands_admin_CommandPlayerTime)
- [/resourceworld](#commands_admin_CommandResourceWorld)
- [/royalsword](#commands_admin_CommandRoyalSword)
- [/sc](#commands_admin_CommandStaffChat)
- [/scripts](#commands_admin_CommandScripts)
- [/sign](#commands_admin_CommandSign)
- [/skull](#commands_admin_CommandSkull)
- [/spectator](#commands_admin_CommandSpecificGameMode)
- [/speed](#commands_admin_CommandSpeed)
- [/structfunction](#commands_admin_CommandStructFunction)
- [/sudo](#commands_admin_CommandSudo)
- [/survival](#commands_admin_CommandSpecificGameMode)
- [/teleport](#commands_admin_CommandTeleport)
- [/time](#commands_admin_CommandTime)
- [/top](#commands_admin_CommandTop)
- [/tp_exact](#commands_admin_CommandTeleportExact)
- [/vanish](#commands_admin_CommandVanish)
- [/world](#commands_admin_CommandWorld)

# Commands
## /adventure <a name="commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to adventure  
  
**Command metadata**:  
Permission: `ftc.commands.gamemode.adventure`  
Aliases: `gma`  
### Usages
```yaml
/adventure
# Sets your gamemode to adventure

/adventure <player>
# Sets a <player>'s gamemode to adventure
```

## /broadcast <a name="commands_admin_CommandBroadcast"></a>
Broadcasts a message to the entire server.  
  
**Command metadata**:  
Permission: `ftc.broadcast`  
Aliases: `announce`, `bc`, `ac`  
### Usages
```yaml
/broadcast <message>
# Broadcasts a <message> to the entire server
```

## /cooldown <a name="commands_admin_CommandCooldown"></a>
Controls various cooldowns  
  
**Command metadata**:  
Permission: `ftc.commands.cooldown`  
### Usages
```yaml
/cooldown <user> <category>
# Shows how long a <user> is on cooldown in a <category>

/cooldown <user> <category> add [<length>]
# Adds a <user> into a <category>'s cooldown.
# If <length> is not set, the cooldown will never end

/cooldown <user> <category> remove
# Removes a <user> from a cooldown in a <category>
```

## /creative <a name="commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to creative  
  
**Command metadata**:  
Permission: `ftc.commands.gamemode.creative`  
Aliases: `gmc`  
### Usages
```yaml
/creative
# Sets your gamemode to creative

/creative <player>
# Sets a <player>'s gamemode to creative
```

## /dungeons <a name="commands_admin_CommandDungeons"></a>
Admin command to manage the dungeons  
  
**Command metadata**:  
Permission: `ftc.commands.dungeons`  
### Usages
```yaml
/dungeons spawndummy [<location: x,y,z>]
# Spawns a punching bag
# if [location] is not set, spawns it
# where you're standing

/dungeons debug apples <boss>
# Gives you a <boss>'s golden apple

/dungeons debug <boss> kill
# Kills a boss, if it's alive

/dungeons debug <boss> attemptSpawn
# Attempts to spawn the boss, as if
# a normal player were using the spawn boss
# slime in a boss room

/dungeons debug <boss> spawn
# Spawns the boss, if it
# hasn't already been spawned
```

## /endopener <a name="commands_admin_CommandEndOpener"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  

## /ftcreload <a name="commands_admin_SaveReloadCommands"></a>
Reloads the FTC plugin, or a single module  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/ftcreload
# Reloads the entire FTC plugin

/ftcreload <module>
# Reloads the <module>
```

## /ftcsave <a name="commands_admin_SaveReloadCommands"></a>
Saves the FTC plugin, or a single module  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/ftcsave
# Saves the entire FTC plugin

/ftcsave <module>
# Saves the <module>
```

## /ftcstruct <a name="commands_admin_CommandFtcStruct"></a>
Command to place, create and manage FTC structures  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `ftcstructure`, `structure`, `struct`  
### Usages
```yaml
/ftcstruct create <name>
# Creates a Structure from your selected
# region and gives it the <name>

/ftcstruct create <name> [ignore_blocks=<block tags>] [ignore_entities=<entity type list>] [include_functions=<true | false>]
# Creates a Structure with the given parameters
# -ignore_blocks: A list of blocks that'll be ignored
#   when the Structure is being scanned
# -ignore_entities: A list of entity types that won't be
#   included in the Structure
# -include_functions: Whether to include structure functions
#   in the Structure or not

/ftcstruct <structure name> palette add <name>
# Creates a Palette from your selected
# region and gives it the <name>

/ftcstruct <structure name> palette add <name> [ignore_blocks=<block tags>] [ignore_entities=<entity type list>] [include_functions=<true | false>]
# Creates a Palette with the given parameters
# -ignore_blocks: A list of blocks that'll be ignored
#   when the Palette is being scanned
# -ignore_entities: A list of entity types that won't be
#   included in the Palette
# -include_functions: Whether to include structure functions
#   in the Palette or not

/ftcstruct <structure name> palette remove <name>
# Removes a palette with <name> from a <structure>

/ftcstruct <structure name> place
# Places the structure where you're standing

/ftcstruct <structure name> remove
# Deletes a <structure>

/ftcstruct <structure name> place [rotation=<rot>] [offset=<x,y,z>] [pivot=<x,y,z>] [pos=<x,y,z>] [place_entities=<true | false>] [ignore_air=<true | false>] [palette=<name>]
# Places a <structure> with the parameters
# 
# -rotation: The rotation applied to the structure
# -offset: Offset applied to the structure
# -pivot: The pivot used when placing the structure
# -pos: The position the structure is placed at
# -place_entities: Whether to place entities
# -ignore_air: If true, then existing blocks in the world
#   won't be overridden if they would be overriden by air
# -palette: the name of structure palette to place

/ftcstruct <structure name> header
# Displays the Structure data

/ftcstruct <structure name> header view [<path: nbt path>]
# Displays Structure data, if [path] is set, shows only
# data at that path

/ftcstruct <structure name> header insert <path: nbt path> <tag>
# Inserts a <tag> into Structure data at a <path>

/ftcstruct <structure name> header merge <tag>
# Merges a <tag> into Structure data

/ftcstruct <structure name> header set <tag>
# Completely overwrites the existing Structure data
# and sets it to <tag>
```

## /ftcversion <a name="commands_admin_CommandFtcVersion"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  

## /getoffset <a name="commands_admin_CommandGetOffset"></a>
Gets the offset between 2 selected points  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/getoffset
# Gets the offset between 2 selected points
```

## /getpos <a name="commands_admin_CommandGetPos"></a>
Gets the accurate position of a player  
  
**Command metadata**:  
Permission: `ftc.commands.getpos`  

## /gift <a name="commands_admin_CommandGift"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  

## /gm <a name="commands_admin_CommandGameMode"></a>
Sets your or another player's gamemode  
  
**Command metadata**:  
Permission: `ftc.commands.gamemode`  
Aliases: `gamemode`  
### Usages
```yaml
/gm <game mode>
# Sets your game mode to <game mode>

/gm <game mode> <player>
# Sets a <player>'s game mode to <game mode>
```

## /hologram <a name="commands_admin_CommandHologram"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  

## /illegalworlds <a name="commands_admin_CommandIllegalWorlds"></a>
Command to manage illegal worlds
An illegal world is any world to which a player cannot TP or /home into  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/illegalworlds
# Lists all 'illegal worlds'

/illegalworlds add <world>
# Adds a world to the illegal worlds list

/illegalworlds remove <world>
# Removes a world from the illegal worlds list
```

## /invstore <a name="commands_admin_CommandInvStore"></a>
Lets you give players separate inventories  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/invstore save <player> <category: quoted string> [-doNotClear]
# Saves a <player>'s inventory in a <category>
# If the '-doNotClear' flag is not set, the player's
# inventory is cleared after it's stored away

/invstore return <player> <category: quoted string> [-doNotClear]
# Returns all items a <player> has stored in a <category>
# If the '-doNotClear' flag is not set, the player's inventory
# is cleared before any items are returned
# This command will also remove the items from storage

/invstore swap <player> <category: quoted string>
# Swaps a <player>'s current inventory with the one stored in
# <category>. If the player has no stored inventory in <category>
# then no items are returned.
# In either case, the player's current items are saved in
# the <category>

/invstore give <player> <category: quoted string> [-doNotClear]
# Works like the 'return' argument, except, it doesn't
# remove the items from storage
```

## /joininfo <a name="commands_admin_CommandJoinInfo"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  

## /launch <a name="commands_admin_CommandLaunch"></a>
Rockets a player in a given direction  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `rocket`  
### Usages
```yaml
/launch <entities>
# Launches every selected entity in
# the direction you're looking

/launch <entities> <velocity: x,y,z>
# Sets the velocity of every entity

/launch <entities> add <velocity: x,y,z>
# Adds to the velocity of every entity
```

## /makeaward <a name="commands_admin_CommandMakeAward"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.commands.makeaward`  

## /memory <a name="commands_admin_CommandMemory"></a>
Displays current memory usage information  
  
**Command metadata**:  
Permission: `ftc.commands.memory`  
Aliases: `mem`  
### Usages
```yaml
/memory
# Displays current memory usage information
```

## /npc <a name="commands_admin_CommandNPC"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.commands.npc`  

## /playertime <a name="commands_admin_CommandPlayerTime"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `ptime`  

## /resourceworld <a name="commands_admin_CommandResourceWorld"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `rw`  

## /royalsword <a name="commands_admin_CommandRoyalSword"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.royalsword`  
### Usages
```yaml
/royalsword create <owner: player> [<level>]
# Creates a sword with an <owner>
# If <level> is specified, the sword is upgraded to
# that level

/royalsword update
# Forces your held sword to update
# the lore and sword data, this is
# normally done after killing any mob
# with the sword, or after using a sword's
# ability

/royalsword upgrade
# Upgrades your held sword by 1 level

/royalsword ability
# Shows the active ability of your held sword

/royalsword ability <ability> [<level: number(1..)>]
# Sets the active ability of your held sword
# If <level> is not set, defaults to 1

/royalsword ability cooldown <ticks>
# Adds a cooldown override to the ability of the sword
# you're holding

/royalsword ability cooldown remove_override
# Removes the cooldown override of the sword you're holding

/royalsword ability remaining_uses <uses: number(0..)>
# Sets the remaining uses of the ability of the
# sword you're holding

/royalsword ability remaining_uses infinite
# Sets the remaining uses to 'infinite' for the
# ability of the sword you're holding.
# This means the ability will never run out of uses

/royalsword data
# Displays the Sword data

/royalsword data view [<path: nbt path>]
# Displays Sword data, if [path] is set, shows only
# data at that path

/royalsword data insert <path: nbt path> <tag>
# Inserts a <tag> into Sword data at a <path>

/royalsword data merge <tag>
# Merges a <tag> into Sword data

/royalsword data set <tag>
# Completely overwrites the existing Sword data
# and sets it to <tag>
```

## /sc <a name="commands_admin_CommandStaffChat"></a>
Sends a message to the staff chat  
  
**Command metadata**:  
Permission: `ftc.staffchat`  
Aliases: `staffchat`  
### Usages
```yaml
/sc <message>
# Sends a <message> to the staff chat
```

## /scripts <a name="commands_admin_CommandScripts"></a>
Command to use scripts  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `script`  
### Usages
```yaml
/scripts eval <java script code>
# Runs the given JavaScript code

/scripts run <script file> [args=<args array>] [close_after=<true | false>] [method=<name>]
# Runs the given script file's global function
# If the <args> argument is present, the set string array
# is added into the script.
# If <close_after> is set to 'true' or not set at all, the
# script is closed after execution, else, it stays loaded
# <method> specifies the name of the method to run after
# the global scope has been executed

/scripts delete <script file>
# Deletes a <script file>
```

## /sign <a name="commands_admin_CommandSign"></a>
Allows you to edit a sign  
  
**Command metadata**:  
Permission: `ftc.commands.sign`  
Aliases: `editsign`  
### Usages
```yaml
/sign <pos: x,y,z> clear
# Clears the sign of all text

/sign <pos: x,y,z> copy
# Copies the sign's content

/sign <pos: x,y,z> paste
# Pastes your copied sign contents onto a sign

/sign <pos: x,y,z> <line: number(1..4)> <text>
# Sets a sign's <line> to <text>

/sign <pos: x,y,z> <line: number(1..4)> -clear
# Clears <line>

/sign <pos: x,y,z> type <type>
# Sets the sign's type

/sign <pos: x,y,z> glow <true | false>
# Makes a sign glow/not glow
```

## /skull <a name="commands_admin_CommandSkull"></a>
Gets a player's skull  
  
**Command metadata**:  
Permission: `ftc.commands.skull`  
### Usages
```yaml
/skull <player>
# Gets a <player>'s skull
```

## /spectator <a name="commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to spectator  
  
**Command metadata**:  
Permission: `ftc.commands.gamemode.spectator`  
Aliases: `gmsp`  
### Usages
```yaml
/spectator
# Sets your gamemode to spectator

/spectator <player>
# Sets a <player>'s gamemode to spectator
```

## /speed <a name="commands_admin_CommandSpeed"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/speed walk query
# Queries your walking speed

/speed walk query <player>
# Queries a <player>'s walking speed

/speed walk <value: number(-10, 10)>
# Sets your walking speed

/speed walk <value: number(-10, 10)> <player>
# Sets a <player>'s walking speed

/speed fly query
# Queries your flying speed

/speed fly query <player>
# Queries a <player>'s flying speed

/speed fly <value: number(-10, 10)>
# Sets your flying speed

/speed fly <value: number(-10, 10)> <player>
# Sets a <player>'s flying speed
```

## /structfunction <a name="commands_admin_CommandStructFunction"></a>
Ignore this command  
  
**Command metadata**:  
Permission: `ftc.commands.structfunction`  

## /sudo <a name="commands_admin_CommandSudo"></a>
Forces another user to perform a command or to write in chat  
  
**Command metadata**:  
Permission: `ftc.commands.sudo`  
### Usages
```yaml
/sudo <user> <command>
# Forces a <user> to perform a <command>

/sudo <user> chat:<message>
# Forces a <user> to write in chat
```

## /survival <a name="commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to survival  
  
**Command metadata**:  
Permission: `ftc.commands.gamemode`  
Aliases: `gms`  
### Usages
```yaml
/survival
# Sets your gamemode to survival

/survival <player>
# Sets a <player>'s gamemode to survival
```

## /teleport <a name="commands_admin_CommandTeleport"></a>
FTC's version of the vanilla /tp command  
  
**Command metadata**:  
Permission: `ftc.commands.teleport`  
Aliases: `tp`, `teleport`, `eteleport`, `etp`  

## /time <a name="commands_admin_CommandTime"></a>
Sets the time in your world  
  
**Command metadata**:  
Permission: `ftc.commands.time`  
### Usages
```yaml
/time set <day | noon | night | midnight>
# Sets the time in your world to a 
# corresponding constant

/time set <time: world time>
# Sets the world time

/time add <time: world time>
# Adds to <time> the world's time

/time get [<world>]
# Gets the current world time in [world].
# If [world] is not set, gets the time in
# the world you're in
```

## /top <a name="commands_admin_CommandTop"></a>
Teleports you to the top block in your X and Z pos  
  
**Command metadata**:  
Permission: `ftc.admin`  

## /tp_exact <a name="commands_admin_CommandTeleportExact"></a>
Command for more precise teleportation  
  
**Command metadata**:  
Permission: `ftc.commands.teleport`  
### Usages
```yaml
/tp_exact world=<world> x=<cord> y=<cord> z=<cord> [yaw=<value>] [pitch=<value>]
# Teleports you to the location specified in the parameters
```

## /vanish <a name="commands_admin_CommandVanish"></a>
Makes you or another player vanish  
  
**Command metadata**:  
Permission: `ftc.vanish`  
Aliases: `v`  
### Usages
```yaml
/vanish
# Silently vanishes/unvanishes you

/vanish -joinLeaveMessage
# Vanishes/unvanishes you, and broadcasts a
# Join/leave message

/vanish <player>
# Silently vanishes/unvanishes a <player>

/vanish <player> -joinLeaveMessage
# Vanishes/unvanishes a <player>, and
# broadcasts a Join/leave message
```

## /world <a name="commands_admin_CommandWorld"></a>
Teleports you or another player into a world  
  
**Command metadata**:  
Permission: `ftc.commands.teleport`  
### Usages
```yaml
/world <world>
# Teleports you into a <world>

/world <world> <user>
# Teleports a <user> into a <world>
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Thu Mar 30 22:08:46 CEST 2023`  
Plugin version: `1.19.4-1733-RELEASE`  
Total commands: 40