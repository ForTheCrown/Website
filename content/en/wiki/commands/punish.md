---
title: "Punish"
linkTitle: "Punish"
type: docs
weight: 1
description: >
  Punish Commands
---

# Table of Contents
- [ban](#net_forthecrown_commands_punish_PunishmentCommand)
- [mute](#net_forthecrown_commands_punish_PunishmentCommand)
- [unban](#net_forthecrown_commands_punish_PardonCommand)
- [kick](#net_forthecrown_commands_punish_PunishmentCommand$CommandKick)
- [ipban](#net_forthecrown_commands_punish_PunishmentCommand)
- [notes](#net_forthecrown_commands_punish_CommandNotes)
- [smite](#net_forthecrown_commands_punish_CommandSmite)
- [jail](#net_forthecrown_commands_punish_CommandJail)
- [seperate](#net_forthecrown_commands_punish_CommandSeparate)
- [unbanip](#net_forthecrown_commands_punish_PardonCommand)
- [punish](#net_forthecrown_commands_punish_CommandPunish)
- [jails](#net_forthecrown_commands_punish_CommandJails)
- [unsoftmute](#net_forthecrown_commands_punish_PardonCommand)
- [unjail](#net_forthecrown_commands_punish_PardonCommand)
- [unmute](#net_forthecrown_commands_punish_PardonCommand)
- [softmute](#net_forthecrown_commands_punish_PunishmentCommand)

# Commands
# /ban <a name="net_forthecrown_commands_punish_PunishmentCommand"></a>
Punishes a user with a Ban  
  
Permission: `ftc.punish.ban`  
Aliases: `fban`, `banish`, `fbanish`  
## Usages
```yaml
/ban <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a Ban
# If [length] is not set, the punishment will
# not end automatically
```

# /mute <a name="net_forthecrown_commands_punish_PunishmentCommand"></a>
Punishes a user with a Mute  
  
Permission: `ftc.punish.mute`  
## Usages
```yaml
/mute <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a Mute
# If [length] is not set, the punishment will
# not end automatically
```

# /unban <a name="net_forthecrown_commands_punish_PardonCommand"></a>
Pardons a user, if they've been Banned  
  
Permission: `ftc.punish.ban`  
Aliases: `pardon`, `pardonban`  
## Usages
```yaml
/unban <user>
# Pardons a <user>
```

# /kick <a name="net_forthecrown_commands_punish_PunishmentCommand$CommandKick"></a>
Punishes a user with a Kick  
  
Permission: `ftc.punish.kick`  
Aliases: `fkick`, `kickplayer`  
## Usages
```yaml
/kick <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a Kick
# If [length] is not set, the punishment will
# not end automatically
```

# /ipban <a name="net_forthecrown_commands_punish_PunishmentCommand"></a>
Punishes a user with a IpBan  
  
Permission: `ftc.punish.banip`  
Aliases: `banip`, `fbanip`, `fipban`  
## Usages
```yaml
/ipban <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a IpBan
# If [length] is not set, the punishment will
# not end automatically
```

# /notes <a name="net_forthecrown_commands_punish_CommandNotes"></a>
Shows all admin notes of a player  
  
Permission: `ftc.punish.notes`  
## Usages
```yaml
/notes <user>
# Views a <user>'s staff notes

/notes <user> add <text>
# Adds a staff note to a <user>

/notes <user> remove <index>
# Removes a staff note from a <user>
```

# /smite <a name="net_forthecrown_commands_punish_CommandSmite"></a>
Smites a user lol. This command will deal damage  
  
Permission: `ftc.admin`  
## Usages
```yaml
/smite <user>
# Smites a <user>
```

# /jail <a name="net_forthecrown_commands_punish_CommandJail"></a>
Jails a user  
  
Permission: `ftc.punish.jail`  
## Usages
```yaml
/jail <user> <jail> [length=<length: time>] [reason=<reason>]
# Jails the <user> in the <jail>
# If the [length] is not set, the user will
# be jailed forever.
```

# /seperate <a name="net_forthecrown_commands_punish_CommandSeparate"></a>
Seperates/unseparates 2 players  
  
Permission: `ftc.punish.separate`  
## Usages
```yaml
/seperate <user 1> <user 2>
# Separates/unseparates 2 players
```

# /unbanip <a name="net_forthecrown_commands_punish_PardonCommand"></a>
Pardons a user, if they've been IpBanned  
  
Permission: `ftc.punish.banip`  
Aliases: `pardonip`, `ippardon`, `pardonipban`  
## Usages
```yaml
/unbanip <user>
# Pardons a <user>
```

# /punish <a name="net_forthecrown_commands_punish_CommandPunish"></a>
Opens the punishment menu for a specific user  
  
Permission: `ftc.commands.punish`  
Aliases: `p`  
## Usages
```yaml
/punish
# Opens the punishment menu for a specific user
```

# /jails <a name="net_forthecrown_commands_punish_CommandJails"></a>
Lists all jails  
  
Permission: `ftc.punish.jail`  
Aliases: `jaillist`, `listjails`  
## Usages
```yaml
/jails
# Lists all jails
```

# /unsoftmute <a name="net_forthecrown_commands_punish_PardonCommand"></a>
Pardons a user, if they've been SoftMuted  
  
Permission: `ftc.punish.softmute`  
Aliases: `pardonsoftmute`  
## Usages
```yaml
/unsoftmute <user>
# Pardons a <user>
```

# /unjail <a name="net_forthecrown_commands_punish_PardonCommand"></a>
Pardons a user, if they've been Jailed  
  
Permission: `ftc.punish.jail`  
Aliases: `pardonjail`  
## Usages
```yaml
/unjail <user>
# Pardons a <user>
```

# /unmute <a name="net_forthecrown_commands_punish_PardonCommand"></a>
Pardons a user, if they've been Muted  
  
Permission: `ftc.punish.mute`  
Aliases: `pardonmute`  
## Usages
```yaml
/unmute <user>
# Pardons a <user>
```

# /softmute <a name="net_forthecrown_commands_punish_PunishmentCommand"></a>
Punishes a user with a SoftMute  
  
Permission: `ftc.punish.softmute`  
## Usages
```yaml
/softmute <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a SoftMute
# If [length] is not set, the punishment will
# not end automatically
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Tue Mar 21 15:10:51 EET 2023`  
Plugin version: `1.19.4-1719-SNAPSHOT`  
Total commands: 16