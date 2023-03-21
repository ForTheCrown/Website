---
title: "Admin"
linkTitle: "Admin"
type: docs
weight: 1
description: >
  Admin Commands
---

# Table of Contents
- [cooldown](#net_forthecrown_commands_admin_CommandCooldown)
- [ftcstruct](#net_forthecrown_commands_admin_CommandFtcStruct)
- [dungeons](#net_forthecrown_commands_admin_CommandDungeons)
- [sc](#net_forthecrown_commands_admin_CommandStaffChat)
- [sudo](#net_forthecrown_commands_admin_CommandSudo)
- [endopener](#net_forthecrown_commands_admin_CommandEndOpener)
- [launch](#net_forthecrown_commands_admin_CommandLaunch)
- [illegalworlds](#net_forthecrown_commands_admin_CommandIllegalWorlds)
- [vanish](#net_forthecrown_commands_admin_CommandVanish)
- [joininfo](#net_forthecrown_commands_admin_CommandJoinInfo)
- [ftcversion](#net_forthecrown_commands_admin_CommandFtcVersion)
- [royalsword](#net_forthecrown_commands_admin_CommandRoyalSword)
- [getpos](#net_forthecrown_commands_admin_CommandGetPos)
- [makeaward](#net_forthecrown_commands_admin_CommandMakeAward)
- [memory](#net_forthecrown_commands_admin_CommandMemory)
- [speed](#net_forthecrown_commands_admin_CommandSpeed)
- [npc](#net_forthecrown_commands_admin_CommandNPC)
- [gm](#net_forthecrown_commands_admin_CommandGameMode)
- [time](#net_forthecrown_commands_admin_CommandTime)
- [gift](#net_forthecrown_commands_admin_CommandGift)
- [ftcsave](#net_forthecrown_commands_admin_SaveReloadCommands)
- [creative](#net_forthecrown_commands_admin_CommandSpecificGameMode)
- [broadcast](#net_forthecrown_commands_admin_CommandBroadcast)
- [world](#net_forthecrown_commands_admin_CommandWorld)
- [top](#net_forthecrown_commands_admin_CommandTop)
- [spectator](#net_forthecrown_commands_admin_CommandSpecificGameMode)
- [getoffset](#net_forthecrown_commands_admin_CommandGetOffset)
- [sign](#net_forthecrown_commands_admin_CommandSign)
- [teleport](#net_forthecrown_commands_admin_CommandTeleport)
- [survival](#net_forthecrown_commands_admin_CommandSpecificGameMode)
- [adventure](#net_forthecrown_commands_admin_CommandSpecificGameMode)
- [ftcreload](#net_forthecrown_commands_admin_SaveReloadCommands)
- [invstore](#net_forthecrown_commands_admin_CommandInvStore)
- [hologram](#net_forthecrown_commands_admin_CommandHologram)
- [playertime](#net_forthecrown_commands_admin_CommandPlayerTime)
- [tp_exact](#net_forthecrown_commands_admin_CommandTeleportExact)
- [skull](#net_forthecrown_commands_admin_CommandSkull)
- [scripts](#net_forthecrown_commands_admin_CommandScripts)
- [resourceworld](#net_forthecrown_commands_admin_CommandResourceWorld)
- [structfunction](#net_forthecrown_commands_admin_CommandStructFunction)

# Commands
# /cooldown <a name="net_forthecrown_commands_admin_CommandCooldown"></a>
Controls various cooldowns  
  
Permission: `ftc.commands.cooldown`  
## Usages
```yaml
/cooldown <user> <category>
# Shows how long a <user> is on cooldown in a <category>

/cooldown <user> <category> add [<length>]
# Adds a <user> into a <category>'s cooldown.
# If <length> is not set, the cooldown will never end

/cooldown <user> <category> remove
# Removes a <user> from a cooldown in a <category>
```

# /ftcstruct <a name="net_forthecrown_commands_admin_CommandFtcStruct"></a>
Command to place, create and manage FTC structures  
  
Permission: `ftc.admin`  
Aliases: `ftcstructure`, `structure`, `struct`  
## Usages
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

# /dungeons <a name="net_forthecrown_commands_admin_CommandDungeons"></a>
Admin command to manage the dungeons  
  
Permission: `ftc.commands.dungeons`  
## Usages
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

# /sc <a name="net_forthecrown_commands_admin_CommandStaffChat"></a>
Sends a message to the staff chat  
  
Permission: `ftc.staffchat`  
Aliases: `staffchat`  
## Usages
```yaml
/sc <message>
# Sends a <message> to the staff chat
```

# /sudo <a name="net_forthecrown_commands_admin_CommandSudo"></a>
Forces another user to perform a command or to write in chat  
  
Permission: `ftc.commands.sudo`  
## Usages
```yaml
/sudo <user> <command>
# Forces a <user> to perform a <command>

/sudo <user> chat:<message>
# Forces a <user> to write in chat
```

# /endopener <a name="net_forthecrown_commands_admin_CommandEndOpener"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  

# /launch <a name="net_forthecrown_commands_admin_CommandLaunch"></a>
Rockets a player in a given direction  
  
Permission: `ftc.admin`  
Aliases: `rocket`  
## Usages
```yaml
/launch <entities>
# Launches every selected entity in
# the direction you're looking

/launch <entities> <velocity: x,y,z>
# Sets the velocity of every entity

/launch <entities> add <velocity: x,y,z>
# Adds to the velocity of every entity
```

# /illegalworlds <a name="net_forthecrown_commands_admin_CommandIllegalWorlds"></a>
Command to manage illegal worlds
An illegal world is any world to which a player cannot TP or /home into  
  
Permission: `ftc.admin`  
## Usages
```yaml
/illegalworlds
# Lists all 'illegal worlds'

/illegalworlds add <world>
# Adds a world to the illegal worlds list

/illegalworlds remove <world>
# Removes a world from the illegal worlds list
```

# /vanish <a name="net_forthecrown_commands_admin_CommandVanish"></a>
Makes you or another player vanish  
  
Permission: `ftc.vanish`  
Aliases: `v`  
## Usages
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

# /joininfo <a name="net_forthecrown_commands_admin_CommandJoinInfo"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  

# /ftcversion <a name="net_forthecrown_commands_admin_CommandFtcVersion"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  

# /royalsword <a name="net_forthecrown_commands_admin_CommandRoyalSword"></a>
An FTC command (default description)  
  
Permission: `ftc.royalsword`  
## Usages
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

# /getpos <a name="net_forthecrown_commands_admin_CommandGetPos"></a>
Gets the accurate position of a player  
  
Permission: `ftc.commands.getpos`  

# /makeaward <a name="net_forthecrown_commands_admin_CommandMakeAward"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.makeaward`  

# /memory <a name="net_forthecrown_commands_admin_CommandMemory"></a>
Displays current memory usage information  
  
Permission: `ftc.commands.memory`  
Aliases: `mem`  
## Usages
```yaml
/memory
# Displays current memory usage information
```

# /speed <a name="net_forthecrown_commands_admin_CommandSpeed"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  

# /npc <a name="net_forthecrown_commands_admin_CommandNPC"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.npc`  

# /gm <a name="net_forthecrown_commands_admin_CommandGameMode"></a>
Sets your or another player's gamemode  
  
Permission: `ftc.commands.gamemode`  
Aliases: `gamemode`  
## Usages
```yaml
/gm <game mode>
# Sets your game mode to <game mode>

/gm <game mode> <player>
# Sets a <player>'s game mode to <game mode>
```

# /time <a name="net_forthecrown_commands_admin_CommandTime"></a>
Sets the time in your world  
  
Permission: `ftc.commands.time`  
## Usages
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

# /gift <a name="net_forthecrown_commands_admin_CommandGift"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  

# /ftcsave <a name="net_forthecrown_commands_admin_SaveReloadCommands"></a>
Saves the FTC plugin, or a single module  
  
Permission: `ftc.admin`  
## Usages
```yaml
/ftcsave
# Saves the entire FTC plugin

/ftcsave <module>
# Saves the <module>
```

# /creative <a name="net_forthecrown_commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to creative  
  
Permission: `ftc.commands.gamemode.creative`  
Aliases: `gmc`  
## Usages
```yaml
/creative
# Sets your gamemode to creative

/creative <player>
# Sets a <player>'s gamemode to creative
```

# /broadcast <a name="net_forthecrown_commands_admin_CommandBroadcast"></a>
Broadcasts a message to the entire server.  
  
Permission: `ftc.broadcast`  
Aliases: `announce`, `bc`, `ac`  
## Usages
```yaml
/broadcast <message>
# Broadcasts a <message> to the entire server
```

# /world <a name="net_forthecrown_commands_admin_CommandWorld"></a>
Teleports you or another player into a world  
  
Permission: `ftc.commands.teleport`  
## Usages
```yaml
/world <world>
# Teleports you into a <world>

/world <world> <user>
# Teleports a <user> into a <world>
```

# /top <a name="net_forthecrown_commands_admin_CommandTop"></a>
Teleports you to the top block in your X and Z pos  
  
Permission: `ftc.admin`  

# /spectator <a name="net_forthecrown_commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to spectator  
  
Permission: `ftc.commands.gamemode.spectator`  
Aliases: `gmsp`  
## Usages
```yaml
/spectator
# Sets your gamemode to spectator

/spectator <player>
# Sets a <player>'s gamemode to spectator
```

# /getoffset <a name="net_forthecrown_commands_admin_CommandGetOffset"></a>
Gets the offset between 2 selected points  
  
Permission: `ftc.admin`  
## Usages
```yaml
/getoffset
# Gets the offset between 2 selected points
```

# /sign <a name="net_forthecrown_commands_admin_CommandSign"></a>
Allows you to edit a sign  
  
Permission: `ftc.commands.sign`  
Aliases: `editsign`  
## Usages
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

# /teleport <a name="net_forthecrown_commands_admin_CommandTeleport"></a>
FTC's version of the vanilla /tp command  
  
Permission: `ftc.commands.teleport`  
Aliases: `tp`, `teleport`, `eteleport`, `etp`  

# /survival <a name="net_forthecrown_commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to survival  
  
Permission: `ftc.commands.gamemode`  
Aliases: `gms`  
## Usages
```yaml
/survival
# Sets your gamemode to survival

/survival <player>
# Sets a <player>'s gamemode to survival
```

# /adventure <a name="net_forthecrown_commands_admin_CommandSpecificGameMode"></a>
Sets your gamemode to adventure  
  
Permission: `ftc.commands.gamemode.adventure`  
Aliases: `gma`  
## Usages
```yaml
/adventure
# Sets your gamemode to adventure

/adventure <player>
# Sets a <player>'s gamemode to adventure
```

# /ftcreload <a name="net_forthecrown_commands_admin_SaveReloadCommands"></a>
Reloads the FTC plugin, or a single module  
  
Permission: `ftc.admin`  
## Usages
```yaml
/ftcreload
# Reloads the entire FTC plugin

/ftcreload <module>
# Reloads the <module>
```

# /invstore <a name="net_forthecrown_commands_admin_CommandInvStore"></a>
Lets you give players separate inventories  
  
Permission: `ftc.admin`  
## Usages
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

# /hologram <a name="net_forthecrown_commands_admin_CommandHologram"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  

# /playertime <a name="net_forthecrown_commands_admin_CommandPlayerTime"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
Aliases: `ptime`  

# /tp_exact <a name="net_forthecrown_commands_admin_CommandTeleportExact"></a>
Command for more precise teleportation  
  
Permission: `ftc.commands.teleport`  
## Usages
```yaml
/tp_exact world=<world> x=<cord> y=<cord> z=<cord> [yaw=<value>] [pitch=<value>]
# Teleports you to the location specified in the parameters
```

# /skull <a name="net_forthecrown_commands_admin_CommandSkull"></a>
Gets a player's skull  
  
Permission: `ftc.commands.skull`  
## Usages
```yaml
/skull <player>
# Gets a <player>'s skull
```

# /scripts <a name="net_forthecrown_commands_admin_CommandScripts"></a>
Command to use scripts  
  
Permission: `ftc.admin`  
Aliases: `script`  
## Usages
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

# /resourceworld <a name="net_forthecrown_commands_admin_CommandResourceWorld"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
Aliases: `rw`  

# /structfunction <a name="net_forthecrown_commands_admin_CommandStructFunction"></a>
Ignore this command  
  
Permission: `ftc.commands.structfunction`  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Tue Mar 21 15:10:51 EET 2023`  
Plugin version: `1.19.4-1719-SNAPSHOT`  
Total commands: 40