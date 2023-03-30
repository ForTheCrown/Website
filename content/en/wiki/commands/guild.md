---
title: "Guild"
linkTitle: "Guild"
type: docs
weight: 1
description: >
  Guild Commands
---

# Table of Contents
- [/g chat](#commands_guild_GuildChatNode)
- [/g chunks](#commands_guild_GuildChunkNode)
- [/g create](#commands_guild_GuildCreateNode)
- [/g delete](#commands_guild_GuildDeleteNode)
- [/g demote](#commands_guild_GuildChangeRankNode)
- [/g discover](#commands_guild_GuildDiscoveryNode)
- [/g help](#commands_guild_GuildHelpNode)
- [/g info](#commands_guild_GuildInfoNode)
- [/g inventory](#commands_guild_GuildInventoryNode)
- [/g invite](#commands_guild_GuildInviteNode)
- [/g join](#commands_guild_GuildJoinNode)
- [/g kick](#commands_guild_GuildKickNode)
- [/g l](#commands_guild_GuildListNode)
- [/g leave](#commands_guild_GuildLeaveNode)
- [/g multiplier](#commands_guild_GuildMultiplierNode)
- [/g promote](#commands_guild_GuildChangeRankNode)
- [/g set](#commands_guild_GuildSetNode)
- [/g toggleperm](#commands_guild_GuildPermNode)
- [/guild](#commands_guild_GuildCommands$CommandGuild)

# Commands
## /g chat <a name="commands_guild_GuildChatNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `gc`  
### Usages
```yaml
/g chat <message>
# Sends a message into the guild chat

/g chat <guild> <message>
# Sends a message into a guild's chat
```

## /g chunks <a name="commands_guild_GuildChunkNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g chunks list
# Displays thechunks your guild owns

/g chunks claim
# Claims the chunk you're in for your guild

/g chunks unclaim
# Unclaims the chunk you're in for your guild

/g chunks unclaimall
# Unclaims ALL chunks owned by your guild

/g chunks list <guild>
# List the chunks of a guild

/g chunks claim <guild
# Claims the chunk you're in for a guild

/g chunks unclaim <guild>
# Unclaims the chunk you're in for a guild

/g chunks unclaimall <guild>
# Unclaims all the chunks of a guild
```

## /g create <a name="commands_guild_GuildCreateNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `createguild`, `gcreate`  
### Usages
```yaml
/g create <name>
# Creates a new guild with the name
```

## /g delete <a name="commands_guild_GuildDeleteNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `guilddelete`, `gdelete`  
### Usages
```yaml
/g delete
# Deletes your guild

/g delete <guild>
# Deletes a guild
```

## /g demote <a name="commands_guild_GuildChangeRankNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g demote <user>
# Demotes a user

/g demote <user> <guild>
# Demotes a user in a guild
```

## /g discover <a name="commands_guild_GuildDiscoveryNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `discoverguilds`, `guilddiscovery`, `gdiscover`  
### Usages
```yaml
/g discover
# Opens a menu to find guilds to join
```

## /g help <a name="commands_guild_GuildHelpNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `ghelp`  
### Usages
```yaml
/g help
# Shows help information
```

## /g info <a name="commands_guild_GuildInfoNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g info
# Displays info about your guild

/g info <guild>
# Displays info about a specific guild
```

## /g inventory <a name="commands_guild_GuildInventoryNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `ginv`, `guildinv`  
### Usages
```yaml
/g inventory
# Opens your guild's inventory

/g inventory <guild>
# Opens a <guild>'s inventory
```

## /g invite <a name="commands_guild_GuildInviteNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g invite <user>
# Invites a player to your guild

/g invite <user> cancel
# Cancels a sent invite

/g invite accept <guild>
# Accepts a guild join invite

/g invite deny <guild>
# Denies a guild join invite
```

## /g join <a name="commands_guild_GuildJoinNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g join <guild>
# Joins a guild
```

## /g kick <a name="commands_guild_GuildKickNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g kick <user>
# Kicks a user out of your guild

/g kick <user> <guild>
# Kicks a user out of a guild
```

## /g l <a name="commands_guild_GuildListNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `guildlist`, `glist`  
### Usages
```yaml
/g l
# Lists all guilds
```

## /g leave <a name="commands_guild_GuildLeaveNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g leave
# Leaves the current guild you're in
```

## /g multiplier <a name="commands_guild_GuildMultiplierNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g multiplier
# Opens the multiplier menu

/g multiplier add player=<player> type=<guild | global> length=<time> value=<multiplier>
# Adds a multiplier

/g multiplier manual
# Shows the current manual modifier

/g multiplier manual <value: number(0..)>
# Sets the current manual modifier to a <value>

/g multiplier <player> <type: global | guild>
# Lists all <type> multipliers a <player> has

/g multiplier <player> <type: global | guild> remove <index>
# Removes a <type> multiplier from <player>.
# Use /g multiplier <player> <type> to list a <player>'s
# multipliers

/g multiplier <player> <type: global | guild> clear
# Clears all <type> multipliers a <player> has
```

## /g promote <a name="commands_guild_GuildChangeRankNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
### Usages
```yaml
/g promote <user>
# Promotes a user

/g promote <user> <guild>
# Promotes a user in a guild
```

## /g set <a name="commands_guild_GuildSetNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `gset`  
### Usages
```yaml
/g set name <name>
# Sets your guild's name

/g set leader <player>
# Sets your guild's leader

/g set waypoint
# Sets your guild's waypoint to the waypoint you're looking
# at, or the closest one to you

/g set discordAnnouncements
# Sets whether guild announcements are
# forwarded to the guild's discord channel

/g set unlimitedMembers <guild> <true | false>
# Sets whether a guild can have unlimited members

/g set unlimitedMembers <guild>
# Checks whether a guild has unlimited members.

/g set unlimitedChunks <guild> <true | false>
# Sets whether a guild can have unlimited chunks

/g set unlimitedChunks <guild>
# Checks whether a guild has unlimited chunks.
```

## /g toggleperm <a name="commands_guild_GuildPermNode"></a>
Guild command, see '/help guild' for more info  
  
**Command metadata**:  
Permission: `ftc.guild`  

## /guild <a name="commands_guild_GuildCommands$CommandGuild"></a>
Guild command  
  
**Command metadata**:  
Permission: `ftc.guild`  
Aliases: `g`  
### Usages
```yaml
/guild help
# Shows help information

/guild info
# Displays info about your guild

/guild info <guild>
# Displays info about a specific guild

/guild l
# Lists all guilds

/guild set name <name>
# Sets your guild's name

/guild set leader <player>
# Sets your guild's leader

/guild set waypoint
# Sets your guild's waypoint to the waypoint you're looking
# at, or the closest one to you

/guild set discordAnnouncements
# Sets whether guild announcements are
# forwarded to the guild's discord channel

/guild set unlimitedMembers <guild> <true | false>
# Sets whether a guild can have unlimited members

/guild set unlimitedMembers <guild>
# Checks whether a guild has unlimited members.

/guild set unlimitedChunks <guild> <true | false>
# Sets whether a guild can have unlimited chunks

/guild set unlimitedChunks <guild>
# Checks whether a guild has unlimited chunks.

/guild invite <user>
# Invites a player to your guild

/guild invite <user> cancel
# Cancels a sent invite

/guild invite accept <guild>
# Accepts a guild join invite

/guild invite deny <guild>
# Denies a guild join invite

/guild kick <user>
# Kicks a user out of your guild

/guild kick <user> <guild>
# Kicks a user out of a guild

/guild join <guild>
# Joins a guild

/guild leave
# Leaves the current guild you're in

/guild chunks list
# Displays thechunks your guild owns

/guild chunks claim
# Claims the chunk you're in for your guild

/guild chunks unclaim
# Unclaims the chunk you're in for your guild

/guild chunks unclaimall
# Unclaims ALL chunks owned by your guild

/guild chunks list <guild>
# List the chunks of a guild

/guild chunks claim <guild
# Claims the chunk you're in for a guild

/guild chunks unclaim <guild>
# Unclaims the chunk you're in for a guild

/guild chunks unclaimall <guild>
# Unclaims all the chunks of a guild

/guild chat <message>
# Sends a message into the guild chat

/guild chat <guild> <message>
# Sends a message into a guild's chat

/guild inventory
# Opens your guild's inventory

/guild inventory <guild>
# Opens a <guild>'s inventory

/guild create <name>
# Creates a new guild with the name

/guild delete
# Deletes your guild

/guild delete <guild>
# Deletes a guild

/guild discover
# Opens a menu to find guilds to join

/guild multiplier
# Opens the multiplier menu

/guild multiplier add player=<player> type=<guild | global> length=<time> value=<multiplier>
# Adds a multiplier

/guild multiplier manual
# Shows the current manual modifier

/guild multiplier manual <value: number(0..)>
# Sets the current manual modifier to a <value>

/guild multiplier <player> <type: global | guild>
# Lists all <type> multipliers a <player> has

/guild multiplier <player> <type: global | guild> remove <index>
# Removes a <type> multiplier from <player>.
# Use /g multiplier <player> <type> to list a <player>'s
# multipliers

/guild multiplier <player> <type: global | guild> clear
# Clears all <type> multipliers a <player> has

/guild promote <user>
# Promotes a user

/guild promote <user> <guild>
# Promotes a user in a guild

/guild demote <user>
# Demotes a user

/guild demote <user> <guild>
# Demotes a user in a guild
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Thu Mar 30 22:08:46 CEST 2023`  
Plugin version: `1.19.4-1733-RELEASE`  
Total commands: 19