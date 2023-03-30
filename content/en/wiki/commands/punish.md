---
title: "Punish"
linkTitle: "Punish"
type: docs
weight: 1
description: >
  Punish Commands
---

# Table of Contents
- [/ban](#commands_punish_PunishmentCommand)
- [/ipban](#commands_punish_PunishmentCommand)
- [/jail](#commands_punish_CommandJail)
- [/jails](#commands_punish_CommandJails)
- [/kick](#commands_punish_PunishmentCommand$CommandKick)
- [/mute](#commands_punish_PunishmentCommand)
- [/notes](#commands_punish_CommandNotes)
- [/punish](#commands_punish_CommandPunish)
- [/seperate](#commands_punish_CommandSeparate)
- [/smite](#commands_punish_CommandSmite)
- [/softmute](#commands_punish_PunishmentCommand)
- [/unban](#commands_punish_PardonCommand)
- [/unbanip](#commands_punish_PardonCommand)
- [/unjail](#commands_punish_PardonCommand)
- [/unmute](#commands_punish_PardonCommand)
- [/unsoftmute](#commands_punish_PardonCommand)

# Commands
## /ban <a name="commands_punish_PunishmentCommand"></a>
Punishes a user with a Ban  
  
**Command metadata**:  
Permission: `ftc.punish.ban`  
Aliases: `fban`, `banish`, `fbanish`  
### Usages
```yaml
/ban <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a Ban
# If [length] is not set, the punishment will
# not end automatically
```

## /ipban <a name="commands_punish_PunishmentCommand"></a>
Punishes a user with a IpBan  
  
**Command metadata**:  
Permission: `ftc.punish.banip`  
Aliases: `banip`, `fbanip`, `fipban`  
### Usages
```yaml
/ipban <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a IpBan
# If [length] is not set, the punishment will
# not end automatically
```

## /jail <a name="commands_punish_CommandJail"></a>
Jails a user  
  
**Command metadata**:  
Permission: `ftc.punish.jail`  
### Usages
```yaml
/jail <user> <jail> [length=<length: time>] [reason=<reason>]
# Jails the <user> in the <jail>
# If the [length] is not set, the user will
# be jailed forever.
```

## /jails <a name="commands_punish_CommandJails"></a>
Lists all jails  
  
**Command metadata**:  
Permission: `ftc.punish.jail`  
Aliases: `jaillist`, `listjails`  
### Usages
```yaml
/jails
# Lists all jails
```

## /kick <a name="commands_punish_PunishmentCommand$CommandKick"></a>
Punishes a user with a Kick  
  
**Command metadata**:  
Permission: `ftc.punish.kick`  
Aliases: `fkick`, `kickplayer`  
### Usages
```yaml
/kick <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a Kick
# If [length] is not set, the punishment will
# not end automatically
```

## /mute <a name="commands_punish_PunishmentCommand"></a>
Punishes a user with a Mute  
  
**Command metadata**:  
Permission: `ftc.punish.mute`  
### Usages
```yaml
/mute <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a Mute
# If [length] is not set, the punishment will
# not end automatically
```

## /notes <a name="commands_punish_CommandNotes"></a>
Shows all admin notes of a player  
  
**Command metadata**:  
Permission: `ftc.punish.notes`  
### Usages
```yaml
/notes <user>
# Views a <user>'s staff notes

/notes <user> add <text>
# Adds a staff note to a <user>

/notes <user> remove <index>
# Removes a staff note from a <user>
```

## /punish <a name="commands_punish_CommandPunish"></a>
Opens the punishment menu for a specific user  
  
**Command metadata**:  
Permission: `ftc.commands.punish`  
Aliases: `p`  
### Usages
```yaml
/punish
# Opens the punishment menu for a specific user
```

## /seperate <a name="commands_punish_CommandSeparate"></a>
Seperates/unseparates 2 players  
  
**Command metadata**:  
Permission: `ftc.punish.separate`  
### Usages
```yaml
/seperate <user 1> <user 2>
# Separates/unseparates 2 players
```

## /smite <a name="commands_punish_CommandSmite"></a>
Smites a user lol. This command will deal damage  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/smite <user>
# Smites a <user>
```

## /softmute <a name="commands_punish_PunishmentCommand"></a>
Punishes a user with a SoftMute  
  
**Command metadata**:  
Permission: `ftc.punish.softmute`  
### Usages
```yaml
/softmute <user> [reason=<reason>] [length=<length: time>]
# Punishes a user with a SoftMute
# If [length] is not set, the punishment will
# not end automatically
```

## /unban <a name="commands_punish_PardonCommand"></a>
Pardons a user, if they've been Banned  
  
**Command metadata**:  
Permission: `ftc.punish.ban`  
Aliases: `pardon`, `pardonban`  
### Usages
```yaml
/unban <user>
# Pardons a <user>
```

## /unbanip <a name="commands_punish_PardonCommand"></a>
Pardons a user, if they've been IpBanned  
  
**Command metadata**:  
Permission: `ftc.punish.banip`  
Aliases: `pardonip`, `ippardon`, `pardonipban`  
### Usages
```yaml
/unbanip <user>
# Pardons a <user>
```

## /unjail <a name="commands_punish_PardonCommand"></a>
Pardons a user, if they've been Jailed  
  
**Command metadata**:  
Permission: `ftc.punish.jail`  
Aliases: `pardonjail`  
### Usages
```yaml
/unjail <user>
# Pardons a <user>
```

## /unmute <a name="commands_punish_PardonCommand"></a>
Pardons a user, if they've been Muted  
  
**Command metadata**:  
Permission: `ftc.punish.mute`  
Aliases: `pardonmute`  
### Usages
```yaml
/unmute <user>
# Pardons a <user>
```

## /unsoftmute <a name="commands_punish_PardonCommand"></a>
Pardons a user, if they've been SoftMuted  
  
**Command metadata**:  
Permission: `ftc.punish.softmute`  
Aliases: `pardonsoftmute`  
### Usages
```yaml
/unsoftmute <user>
# Pardons a <user>
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Thu Mar 30 22:08:46 CEST 2023`  
Plugin version: `1.19.4-1733-RELEASE`  
Total commands: 16