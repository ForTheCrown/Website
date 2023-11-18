---
title: "admin"
linkTitle: "admin"
type: docs
weight: 1
description: >
  admin commands
---


## /adventure
Sets your gamemode to adventure  
  
**Permission**: `ftc.commands.gamemode.adventure`  
**Aliases**: `gma`  
**Uses**:
- <pre class="command-usage-arguments">/adventure</pre>  
  Sets your gamemode to adventure  
- <pre class="command-usage-arguments">/adventure &lt;player&gt;</pre>  
  Sets a player's gamemode to adventure  

## /alts
Modify user alt accounts  
  
**Permission**: `ftc.commands.alts`  
**Aliases**: `useralts`, `user_alts`  
**Uses**:
- <pre class="command-usage-arguments">/alts info &lt;user&gt;</pre>  
  Shows alt account info relating to a user  
- <pre class="command-usage-arguments">/alts add &lt;alt&gt; &lt;main&gt;</pre>  
  Marks an alt player as an alt account for a main  
- <pre class="command-usage-arguments">/alts remove &lt;alt&gt; &lt;main&gt;</pre>  
  Removes an alt account from a main account  
- <pre class="command-usage-arguments">/alts clear &lt;main&gt;</pre>  
  Clears all alt account links from a main account  

## /broadcast
Broadcasts a message to the entire server.  
  
**Permission**: `ftc.commands.broadcast`  
**Aliases**: `announce`, `bc`, `ac`  
**Uses**:
- <pre class="command-usage-arguments">/broadcast &lt;message&gt;</pre>  
  Broadcasts a message to the entire server  

## /cooldown
Controls various cooldowns  
  
**Permission**: `ftc.commands.Cooldown`  
**Uses**:
- <pre class="command-usage-arguments">/cooldown &lt;user&gt; &lt;category&gt;</pre>  
  Shows how long a user is on cooldown in a category  
- <pre class="command-usage-arguments">/cooldown &lt;user&gt; &lt;category&gt; add [&lt;length&gt;]</pre>  
  Adds a user into a category's cooldown.  
  If length is not set, the cooldown will never end  
- <pre class="command-usage-arguments">/cooldown &lt;user&gt; &lt;category&gt; remove</pre>  
  Removes a user from a cooldown in a category  

## /creative
Sets your gamemode to creative  
  
**Permission**: `ftc.commands.gamemode.creative`  
**Aliases**: `gmc`  
**Uses**:
- <pre class="command-usage-arguments">/creative</pre>  
  Sets your gamemode to creative  
- <pre class="command-usage-arguments">/creative &lt;player&gt;</pre>  
  Sets a player's gamemode to creative  

## /ftccore
FTC-Core admin command  
  
**Permission**: `ftc.commands.ftccore`  
**Uses**:
- <pre class="command-usage-arguments">/ftccore reload</pre>  
  Reloads the FTC-Core plugin  
- <pre class="command-usage-arguments">/ftccore reload-config</pre>  
  Reloads the FTC-Core config  
- <pre class="command-usage-arguments">/ftccore save</pre>  
  Forces the plugin to save all data  

## /getoffset
Gets the offset between 2 selected points  
  
**Permission**: `ftc.admin`  
**Uses**:
- <pre class="command-usage-arguments">/getoffset</pre>  
  Gets the offset between 2 selected points  

## /getpos
Gets the accurate position of a player  
  
**Permission**: `ftc.commands.getpos`  

## /gm
Sets your or another player's gamemode  
  
**Permission**: `ftc.commands.gamemode`  
**Aliases**: `gamemode`  
**Uses**:
- <pre class="command-usage-arguments">/gm &lt;game mode&gt;</pre>  
  Sets your game mode to game mode  
- <pre class="command-usage-arguments">/gm &lt;game mode&gt; &lt;player&gt;</pre>  
  Sets a player's game mode to game mode  

## /hologram
An FTC command (default description)  
  
**Permission**: `ftc.commands.hologram`  

## /invstore
Lets you give players separate inventories  
  
**Permission**: `ftc.commands.invstore`  
**Uses**:
- <pre class="command-usage-arguments">/invstore reload</pre>  
  Reloads stored inventories  
- <pre class="command-usage-arguments">/invstore save</pre>  
  Saves all currently stored inventories to disk  
- <pre class="command-usage-arguments">/invstore save &lt;player&gt; &lt;category: quoted string&gt; [-doNotClear]</pre>  
  Saves a player's inventory in a category  
  If the '-doNotClear' flag is not set, the player's  
  inventory is cleared after it's stored away  
- <pre class="command-usage-arguments">/invstore return &lt;player&gt; &lt;category: quoted string&gt;</pre>  
  Returns all items a player has stored in a category  
  This command will also remove the items from storage  
- <pre class="command-usage-arguments">/invstore swap &lt;player&gt; &lt;category: quoted string&gt;</pre>  
  Swaps a player's current inventory with the one stored in  
  category. If the player has no stored inventory in category  
  then no items are returned.  
  In either case, the player's current items are saved in  
  the category  
- <pre class="command-usage-arguments">/invstore give &lt;player&gt; &lt;category: quoted string&gt;</pre>  
  Works like the 'return' argument, except, it doesn't  
  remove the items from storage  

## /launch
Rockets a player in a given direction  
  
**Permission**: `ftc.commands.launch`  
**Aliases**: `rocket`  
**Uses**:
- <pre class="command-usage-arguments">/launch &lt;entities&gt;</pre>  
  Launches every selected entity in  
  the direction you're looking  
- <pre class="command-usage-arguments">/launch &lt;entities&gt; &lt;velocity: x,y,z&gt;</pre>  
  Sets the velocity of every entity  
- <pre class="command-usage-arguments">/launch &lt;entities&gt; add &lt;velocity: x,y,z&gt;</pre>  
  Adds to the velocity of every entity  
- <pre class="command-usage-arguments">/launch &lt;entities&gt; at &lt;position: x,y,z&gt; [&lt;multiplier: number&gt;]</pre>  
  Launches all entities towards a specified position  
  multiplier is an optional scalar for the velocity  
- <pre class="command-usage-arguments">/launch &lt;entities&gt; at entity &lt;selector&gt; [&lt;multiplier: number&gt;]</pre>  
  Launches all entities at the selected entities  
  multiplier is an optional scalar for the velocity  

## /makeaward
An FTC command (default description)  
  
**Permission**: `ftc.commands.makeaward`  

## /memory
Displays current memory usage information  
  
**Permission**: `ftc.commands.memory`  
**Aliases**: `mem`  
**Uses**:
- <pre class="command-usage-arguments">/memory</pre>  
  Displays current memory usage information  

## /playertime
Changes the game time for a player  
  
**Permission**: `ftc.admin`  
**Aliases**: `ptime`  

## /sign
Allows you to edit a sign  
  
**Permission**: `ftc.commands.sign`  
**Aliases**: `editsign`  
**Uses**:
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; clear</pre>  
  Clears the sign of all text  
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; copy</pre>  
  Copies the sign's content  
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; paste</pre>  
  Pastes your copied sign contents onto a sign  
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; &lt;line: number(1..4)&gt; &lt;text&gt;</pre>  
  Sets a sign's line to text  
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; &lt;line: number(1..4)&gt; -clear</pre>  
  Clears line  
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; type &lt;type&gt;</pre>  
  Sets the sign's type  
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; glow &lt;true | false&gt;</pre>  
  Makes a sign glow/not glow  
- <pre class="command-usage-arguments">/sign &lt;pos: x,y,z&gt; waxed &lt;true | false&gt;</pre>  
  Sets a sign to be waxed or not  

## /skull
Gets a player's skull  
  
**Permission**: `ftc.commands.skull`  
**Uses**:
- <pre class="command-usage-arguments">/skull &lt;player&gt;</pre>  
  Gets a player's skull  

## /spectator
Sets your gamemode to spectator  
  
**Permission**: `ftc.commands.gamemode.spectator`  
**Aliases**: `gmsp`  
**Uses**:
- <pre class="command-usage-arguments">/spectator</pre>  
  Sets your gamemode to spectator  
- <pre class="command-usage-arguments">/spectator &lt;player&gt;</pre>  
  Sets a player's gamemode to spectator  

## /speed
An FTC command (default description)  
  
**Permission**: `ftc.commands.speed`  
**Uses**:
- <pre class="command-usage-arguments">/speed walk query</pre>  
  Queries your walking speed  
- <pre class="command-usage-arguments">/speed walk query &lt;player&gt;</pre>  
  Queries a player's walking speed  
- <pre class="command-usage-arguments">/speed walk &lt;value: number(-10, 10)&gt;</pre>  
  Sets your walking speed  
- <pre class="command-usage-arguments">/speed walk &lt;value: number(-10, 10)&gt; &lt;player&gt;</pre>  
  Sets a player's walking speed  
- <pre class="command-usage-arguments">/speed fly query</pre>  
  Queries your flying speed  
- <pre class="command-usage-arguments">/speed fly query &lt;player&gt;</pre>  
  Queries a player's flying speed  
- <pre class="command-usage-arguments">/speed fly &lt;value: number(-10, 10)&gt;</pre>  
  Sets your flying speed  
- <pre class="command-usage-arguments">/speed fly &lt;value: number(-10, 10)&gt; &lt;player&gt;</pre>  
  Sets a player's flying speed  

## /survival
Sets your gamemode to survival  
  
**Permission**: `ftc.commands.gamemode`  
**Aliases**: `gms`  
**Uses**:
- <pre class="command-usage-arguments">/survival</pre>  
  Sets your gamemode to survival  
- <pre class="command-usage-arguments">/survival &lt;player&gt;</pre>  
  Sets a player's gamemode to survival  

## /tab
Modifys a player's tab prefix/suffix/display name  
  
**Permission**: `ftc.commands.tab`  
**Aliases**: `user_tab`, `usertab`  
**Uses**:
- <pre class="command-usage-arguments">/tab update</pre>  
  Updates the TAB menu for every player  
- <pre class="command-usage-arguments">/tab name &lt;user&gt; unset</pre>  
  Clears a user's tab display name  
- <pre class="command-usage-arguments">/tab name &lt;user&gt; &lt;text&gt;</pre>  
  Sets a user's tab display name  
- <pre class="command-usage-arguments">/tab prefix &lt;user&gt; unset</pre>  
  Clears a user's tab prefix  
- <pre class="command-usage-arguments">/tab prefix &lt;user&gt; &lt;text&gt;</pre>  
  Sets a user's tab prefix  
- <pre class="command-usage-arguments">/tab suffix &lt;user&gt; unset</pre>  
  Clears a user's tab suffix  
- <pre class="command-usage-arguments">/tab suffix &lt;user&gt; &lt;text&gt;</pre>  
  Sets a user's tab suffix  

## /teleport
Teleports yourself or other entities  
  
**Permission**: `ftc.commands.teleport`  
**Aliases**: `tp`  
**Uses**:
- <pre class="command-usage-arguments">/teleport &lt;location: x,y,z&gt; [&lt;yaw: -180..180&gt;] [&lt;pitch: -90..90&gt;]</pre>  
  Teleports you to a location  
- <pre class="command-usage-arguments">/teleport &lt;entities&gt;</pre>  
  Teleports to an entity  
- <pre class="command-usage-arguments">/teleport &lt;entities&gt; &lt;entity&gt;</pre>  
  Teleports all entities to an entity  
- <pre class="command-usage-arguments">/teleport &lt;entities&gt; &lt;pos: x,y,z&gt;</pre>  
  Teleports all entities to a pos  
- <pre class="command-usage-arguments">/teleport &lt;entities&gt; &lt;pos: x,y,z&gt; &lt;yaw: -180..180&gt; &lt;pitch: -90..90&gt;</pre>  
  Teleports all entities to a location with a set yaw and pitch  
- <pre class="command-usage-arguments">/teleport &lt;entities&gt; &lt;pos: x,y,z&gt; facing entity &lt;facing: entity&gt;</pre>  
  Teleports entities to a location and makes them face an entity  
- <pre class="command-usage-arguments">/teleport &lt;entities&gt; &lt;pos: x,y,z&gt; facing &lt;facing: x,y,z&gt;</pre>  
  Teleports entities to a location and makes them face a position  

## /tellrawf
FTC's version of /tellraw with more lax text input  
  
**Permission**: `ftc.commands.tellrawf`  
**Aliases**: `tellraw`, `ftellraw`, `ftc_tellraw`  

## /time
Sets the time in your world  
  
**Permission**: `ftc.commands.time`  
**Uses**:
- <pre class="command-usage-arguments">/time set &lt;day | noon | night | midnight&gt;</pre>  
  Sets the time in your world to a   
  corresponding constant  
- <pre class="command-usage-arguments">/time set &lt;time: world time&gt;</pre>  
  Sets the world time  
- <pre class="command-usage-arguments">/time add &lt;time: world time&gt;</pre>  
  Adds to time the world's time  
- <pre class="command-usage-arguments">/time get [&lt;world&gt;]</pre>  
  Gets the current world time in [world].  
  If [world] is not set, gets the time in  
  the world you're in  

## /timefield
Allows you to edit users' timestamp fields  
  
**Permission**: `ftc.commands.timefield`  
**Uses**:
- <pre class="command-usage-arguments">/timefield query &lt;user&gt;</pre>  
  Shows a user's time field values  
- <pre class="command-usage-arguments">/timefield query &lt;user&gt; &lt;field&gt;</pre>  
  Shows a specific field's value for a player  
- <pre class="command-usage-arguments">/timefield set &lt;field&gt; &lt;user&gt; present</pre>  
  Sets a time field's value to the present for a player  
- <pre class="command-usage-arguments">/timefield set &lt;field&gt; &lt;user&gt; &lt;value&gt;</pre>  
  Sets a time field's value to a set value  
- <pre class="command-usage-arguments">/timefield unset &lt;field&gt; &lt;user&gt;</pre>  
  Removes a field's value from a player  

## /top
Teleports you to the top block in your X and Z pos  
  
**Permission**: `ftc.commands.teleport`  

## /tp_exact
Command for more precise teleportation  
  
**Permission**: `ftc.commands.teleport`  
**Uses**:
- <pre class="command-usage-arguments">/tp_exact world=&lt;world&gt; x=&lt;cord&gt; y=&lt;cord&gt; z=&lt;cord&gt; [yaw=&lt;value&gt;] [pitch=&lt;value&gt;]</pre>  
  Teleports you to the location specified in the parameters  

## /vanish
Allows staff to become invisible to non-staff  
  
**Permission**: `ftc.vanish`  
**Aliases**: `v`  
**Uses**:
- <pre class="command-usage-arguments">/vanish</pre>  
  Allows staff to become invisible to non-staff  
- <pre class="command-usage-arguments">/vanish silent</pre>  
  Toggles vanish without a join/leave message  
- <pre class="command-usage-arguments">/vanish &lt;other&gt;</pre>  
  Toggles vanish for another player  
- <pre class="command-usage-arguments">/vanish &lt;other&gt; silent</pre>  
  Toggles vanish for another player without announcing a join/leave message  

## /world
Teleports you or another player into a world  
  
**Permission**: `ftc.commands.teleport`  
**Uses**:
- <pre class="command-usage-arguments">/world &lt;world&gt;</pre>  
  Teleports you into a world  
- <pre class="command-usage-arguments">/world &lt;world&gt; &lt;user&gt;</pre>  
  Teleports a user into a world  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 29