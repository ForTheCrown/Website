---
title: "guilds"
linkTitle: "guilds"
type: docs
weight: 1
description: >
  guilds commands
---


## /g chat
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `gc`  
**Uses**:
- <pre class="command-usage-arguments">/g chat &lt;message&gt;</pre>  
  Sends a message into the guild chat  
- <pre class="command-usage-arguments">/g chat &lt;guild&gt; &lt;message&gt;</pre>  
  Sends a message into a guild's chat  

## /g chunks
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g chunks list</pre>  
  Displays thechunks your guild owns  
- <pre class="command-usage-arguments">/g chunks claim</pre>  
  Claims the chunk you're in for your guild  
- <pre class="command-usage-arguments">/g chunks unclaim</pre>  
  Unclaims the chunk you're in for your guild  
- <pre class="command-usage-arguments">/g chunks unclaimall</pre>  
  Unclaims ALL chunks owned by your guild  
- <pre class="command-usage-arguments">/g chunks list &lt;guild&gt;</pre>  
  List the chunks of a guild  
- <pre class="command-usage-arguments">/g chunks claim &lt;guild</pre>  
  Claims the chunk you're in for a guild  
- <pre class="command-usage-arguments">/g chunks unclaim &lt;guild&gt;</pre>  
  Unclaims the chunk you're in for a guild  
- <pre class="command-usage-arguments">/g chunks unclaimall &lt;guild&gt;</pre>  
  Unclaims all the chunks of a guild  

## /g create
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `createguild`, `gcreate`  
**Uses**:
- <pre class="command-usage-arguments">/g create &lt;name&gt;</pre>  
  Creates a new guild with the name  

## /g delete
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `guilddelete`, `gdelete`  
**Uses**:
- <pre class="command-usage-arguments">/g delete</pre>  
  Deletes your guild  
- <pre class="command-usage-arguments">/g delete &lt;guild&gt;</pre>  
  Deletes a guild  

## /g demote
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g demote &lt;user&gt;</pre>  
  Demotes a user  
- <pre class="command-usage-arguments">/g demote &lt;user&gt; &lt;guild&gt;</pre>  
  Demotes a user in a guild  

## /g discover
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `discoverguilds`, `guilddiscovery`, `gdiscover`  
**Uses**:
- <pre class="command-usage-arguments">/g discover</pre>  
  Opens a menu to find guilds to join  

## /g help
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `ghelp`  
**Uses**:
- <pre class="command-usage-arguments">/g help</pre>  
  Shows help information  

## /g info
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g info</pre>  
  Displays info about your guild  
- <pre class="command-usage-arguments">/g info &lt;guild&gt;</pre>  
  Displays info about a specific guild  

## /g inventory
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `ginv`, `guildinv`  
**Uses**:
- <pre class="command-usage-arguments">/g inventory</pre>  
  Opens your guild's inventory  
- <pre class="command-usage-arguments">/g inventory &lt;guild&gt;</pre>  
  Opens a guild's inventory  

## /g invite
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g invite &lt;user&gt;</pre>  
  Invites a player to your guild  
- <pre class="command-usage-arguments">/g invite &lt;user&gt; cancel</pre>  
  Cancels a sent invite  
- <pre class="command-usage-arguments">/g invite accept &lt;guild&gt;</pre>  
  Accepts a guild join invite  
- <pre class="command-usage-arguments">/g invite deny &lt;guild&gt;</pre>  
  Denies a guild join invite  

## /g join
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g join &lt;guild&gt;</pre>  
  Joins a guild  

## /g kick
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g kick &lt;user&gt;</pre>  
  Kicks a user out of your guild  
- <pre class="command-usage-arguments">/g kick &lt;user&gt; &lt;guild&gt;</pre>  
  Kicks a user out of a guild  

## /g l
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `guildlist`, `glist`  
**Uses**:
- <pre class="command-usage-arguments">/g l</pre>  
  Lists all guilds  

## /g leave
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g leave</pre>  
  Leaves the current guild you're in  

## /g multiplier
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g multiplier</pre>  
  Opens the multiplier menu  
- <pre class="command-usage-arguments">/g multiplier add player=&lt;player&gt; type=&lt;guild | global&gt; length=&lt;time&gt; value=&lt;multiplier&gt;</pre>  
  Adds a multiplier  
- <pre class="command-usage-arguments">/g multiplier manual</pre>  
  Shows the current manual modifier  
- <pre class="command-usage-arguments">/g multiplier manual &lt;value: number(0..)&gt;</pre>  
  Sets the current manual modifier to a value  
- <pre class="command-usage-arguments">/g multiplier &lt;player&gt; &lt;type: global | guild&gt;</pre>  
  Lists all type multipliers a player has  
- <pre class="command-usage-arguments">/g multiplier &lt;player&gt; &lt;type: global | guild&gt; remove &lt;index&gt;</pre>  
  Removes a type multiplier from player.  
  Use /g multiplier player type to list a player's  
  multipliers  
- <pre class="command-usage-arguments">/g multiplier &lt;player&gt; &lt;type: global | guild&gt; clear</pre>  
  Clears all type multipliers a player has  

## /g promote
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Uses**:
- <pre class="command-usage-arguments">/g promote &lt;user&gt;</pre>  
  Promotes a user  
- <pre class="command-usage-arguments">/g promote &lt;user&gt; &lt;guild&gt;</pre>  
  Promotes a user in a guild  

## /g set
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  
**Aliases**: `gset`  
**Uses**:
- <pre class="command-usage-arguments">/g set name &lt;name&gt;</pre>  
  Sets your guild's name  
- <pre class="command-usage-arguments">/g set leader &lt;player&gt;</pre>  
  Sets your guild's leader  
- <pre class="command-usage-arguments">/g set discordAnnouncements</pre>  
  Sets whether guild announcements are  
  forwarded to the guild's discord channel  
- <pre class="command-usage-arguments">/g set unlimitedMembers &lt;guild&gt; &lt;true | false&gt;</pre>  
  Sets whether a guild can have unlimited members  
- <pre class="command-usage-arguments">/g set unlimitedMembers &lt;guild&gt;</pre>  
  Checks whether a guild has unlimited members.  
- <pre class="command-usage-arguments">/g set unlimitedChunks &lt;guild&gt; &lt;true | false&gt;</pre>  
  Sets whether a guild can have unlimited chunks  
- <pre class="command-usage-arguments">/g set unlimitedChunks &lt;guild&gt;</pre>  
  Checks whether a guild has unlimited chunks.  

## /g toggleperm
Guild command, see '/help guild' for more info  
  
**Permission**: `ftc.guild`  

## /guild
Guild command  
  
**Permission**: `ftc.guild`  
**Aliases**: `g`  
**Uses**:
- <pre class="command-usage-arguments">/guild reload</pre>  
  Reloads the Guilds plugin  
- <pre class="command-usage-arguments">/guild reload-config</pre>  
  Reloads the Guilds config  
- <pre class="command-usage-arguments">/guild help</pre>  
  Shows help information  
- <pre class="command-usage-arguments">/guild info</pre>  
  Displays info about your guild  
- <pre class="command-usage-arguments">/guild info &lt;guild&gt;</pre>  
  Displays info about a specific guild  
- <pre class="command-usage-arguments">/guild l</pre>  
  Lists all guilds  
- <pre class="command-usage-arguments">/guild set name &lt;name&gt;</pre>  
  Sets your guild's name  
- <pre class="command-usage-arguments">/guild set leader &lt;player&gt;</pre>  
  Sets your guild's leader  
- <pre class="command-usage-arguments">/guild set discordAnnouncements</pre>  
  Sets whether guild announcements are  
  forwarded to the guild's discord channel  
- <pre class="command-usage-arguments">/guild set unlimitedMembers &lt;guild&gt; &lt;true | false&gt;</pre>  
  Sets whether a guild can have unlimited members  
- <pre class="command-usage-arguments">/guild set unlimitedMembers &lt;guild&gt;</pre>  
  Checks whether a guild has unlimited members.  
- <pre class="command-usage-arguments">/guild set unlimitedChunks &lt;guild&gt; &lt;true | false&gt;</pre>  
  Sets whether a guild can have unlimited chunks  
- <pre class="command-usage-arguments">/guild set unlimitedChunks &lt;guild&gt;</pre>  
  Checks whether a guild has unlimited chunks.  
- <pre class="command-usage-arguments">/guild invite &lt;user&gt;</pre>  
  Invites a player to your guild  
- <pre class="command-usage-arguments">/guild invite &lt;user&gt; cancel</pre>  
  Cancels a sent invite  
- <pre class="command-usage-arguments">/guild invite accept &lt;guild&gt;</pre>  
  Accepts a guild join invite  
- <pre class="command-usage-arguments">/guild invite deny &lt;guild&gt;</pre>  
  Denies a guild join invite  
- <pre class="command-usage-arguments">/guild kick &lt;user&gt;</pre>  
  Kicks a user out of your guild  
- <pre class="command-usage-arguments">/guild kick &lt;user&gt; &lt;guild&gt;</pre>  
  Kicks a user out of a guild  
- <pre class="command-usage-arguments">/guild join &lt;guild&gt;</pre>  
  Joins a guild  
- <pre class="command-usage-arguments">/guild leave</pre>  
  Leaves the current guild you're in  
- <pre class="command-usage-arguments">/guild chunks list</pre>  
  Displays thechunks your guild owns  
- <pre class="command-usage-arguments">/guild chunks claim</pre>  
  Claims the chunk you're in for your guild  
- <pre class="command-usage-arguments">/guild chunks unclaim</pre>  
  Unclaims the chunk you're in for your guild  
- <pre class="command-usage-arguments">/guild chunks unclaimall</pre>  
  Unclaims ALL chunks owned by your guild  
- <pre class="command-usage-arguments">/guild chunks list &lt;guild&gt;</pre>  
  List the chunks of a guild  
- <pre class="command-usage-arguments">/guild chunks claim &lt;guild</pre>  
  Claims the chunk you're in for a guild  
- <pre class="command-usage-arguments">/guild chunks unclaim &lt;guild&gt;</pre>  
  Unclaims the chunk you're in for a guild  
- <pre class="command-usage-arguments">/guild chunks unclaimall &lt;guild&gt;</pre>  
  Unclaims all the chunks of a guild  
- <pre class="command-usage-arguments">/guild chat &lt;message&gt;</pre>  
  Sends a message into the guild chat  
- <pre class="command-usage-arguments">/guild chat &lt;guild&gt; &lt;message&gt;</pre>  
  Sends a message into a guild's chat  
- <pre class="command-usage-arguments">/guild inventory</pre>  
  Opens your guild's inventory  
- <pre class="command-usage-arguments">/guild inventory &lt;guild&gt;</pre>  
  Opens a guild's inventory  
- <pre class="command-usage-arguments">/guild create &lt;name&gt;</pre>  
  Creates a new guild with the name  
- <pre class="command-usage-arguments">/guild delete</pre>  
  Deletes your guild  
- <pre class="command-usage-arguments">/guild delete &lt;guild&gt;</pre>  
  Deletes a guild  
- <pre class="command-usage-arguments">/guild discover</pre>  
  Opens a menu to find guilds to join  
- <pre class="command-usage-arguments">/guild multiplier</pre>  
  Opens the multiplier menu  
- <pre class="command-usage-arguments">/guild multiplier add player=&lt;player&gt; type=&lt;guild | global&gt; length=&lt;time&gt; value=&lt;multiplier&gt;</pre>  
  Adds a multiplier  
- <pre class="command-usage-arguments">/guild multiplier manual</pre>  
  Shows the current manual modifier  
- <pre class="command-usage-arguments">/guild multiplier manual &lt;value: number(0..)&gt;</pre>  
  Sets the current manual modifier to a value  
- <pre class="command-usage-arguments">/guild multiplier &lt;player&gt; &lt;type: global | guild&gt;</pre>  
  Lists all type multipliers a player has  
- <pre class="command-usage-arguments">/guild multiplier &lt;player&gt; &lt;type: global | guild&gt; remove &lt;index&gt;</pre>  
  Removes a type multiplier from player.  
  Use /g multiplier player type to list a player's  
  multipliers  
- <pre class="command-usage-arguments">/guild multiplier &lt;player&gt; &lt;type: global | guild&gt; clear</pre>  
  Clears all type multipliers a player has  
- <pre class="command-usage-arguments">/guild promote &lt;user&gt;</pre>  
  Promotes a user  
- <pre class="command-usage-arguments">/guild promote &lt;user&gt; &lt;guild&gt;</pre>  
  Promotes a user in a guild  
- <pre class="command-usage-arguments">/guild demote &lt;user&gt;</pre>  
  Demotes a user  
- <pre class="command-usage-arguments">/guild demote &lt;user&gt; &lt;guild&gt;</pre>  
  Demotes a user in a guild  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 19