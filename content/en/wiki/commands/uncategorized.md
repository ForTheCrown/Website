---
title: "Uncategorized"
linkTitle: "Uncategorized"
type: docs
weight: 1
description: >
  Uncategorized Commands
---

# Table of Contents
- [eavesdrop_muted](#net_forthecrown_commands_ToggleCommand)
- [playtime](#net_forthecrown_commands_UserMapCommand)
- [rank](#net_forthecrown_commands_CommandRank)
- [near](#net_forthecrown_commands_CommandNear)
- [gemtop](#net_forthecrown_commands_UserMapTopCommand)
- [profile](#net_forthecrown_commands_CommandProfile)
- [cartography](#net_forthecrown_commands_ToolBlockCommands)
- [dynmaptoggle](#net_forthecrown_commands_ToggleCommand$1)
- [playerridingtoggle](#net_forthecrown_commands_ToggleCommand$2)
- [topvoters](#net_forthecrown_commands_UserMapTopCommand)
- [nickname](#net_forthecrown_commands_CommandNickname)
- [ftc_me](#net_forthecrown_commands_CommandMe)
- [enderchest](#net_forthecrown_commands_ToolBlockCommands)
- [fly](#net_forthecrown_commands_ToggleCommand)
- [votes](#net_forthecrown_commands_UserMapCommand)
- [marriagechattoggle](#net_forthecrown_commands_ToggleCommand$3)
- [deathtop](#net_forthecrown_commands_CommandLeaderboard)
- [loom](#net_forthecrown_commands_ToolBlockCommands)
- [kittycannon](#net_forthecrown_commands_CommandDumbThing)
- [leave](#net_forthecrown_commands_CommandLeave)
- [hat](#net_forthecrown_commands_CommandHat)
- [workbench](#net_forthecrown_commands_ToolBlockCommands)
- [reply](#net_forthecrown_commands_CommandReply)
- [guildtop](#net_forthecrown_commands_UserMapTopCommand)
- [grindstone](#net_forthecrown_commands_ToolBlockCommands)
- [paytoggle](#net_forthecrown_commands_ToggleCommand)
- [marrytoggle](#net_forthecrown_commands_ToggleCommand)
- [profiletoggle](#net_forthecrown_commands_ToggleCommand)
- [tell](#net_forthecrown_commands_CommandTell)
- [toggleinvites](#net_forthecrown_commands_ToggleCommand)
- [back](#net_forthecrown_commands_CommandBack)
- [rankchat](#net_forthecrown_commands_ToggleCommand)
- [smithingtable](#net_forthecrown_commands_ToolBlockCommands)
- [eavesdrop_dm](#net_forthecrown_commands_ToggleCommand)
- [ignore](#net_forthecrown_commands_CommandIgnore)
- [eavesdrop_mchat](#net_forthecrown_commands_ToggleCommand)
- [afk](#net_forthecrown_commands_CommandAfk)
- [baltop](#net_forthecrown_commands_UserMapTopCommand)
- [balance](#net_forthecrown_commands_UserMapCommand)
- [beezooka](#net_forthecrown_commands_CommandDumbThing)
- [suicide](#net_forthecrown_commands_CommandSuicide)
- [setspawn](#net_forthecrown_commands_CommandSetSpawn)
- [gems](#net_forthecrown_commands_UserMapCommand)
- [staffchattoggle](#net_forthecrown_commands_CommandSelfOrUser)
- [eavesdrop_gchat](#net_forthecrown_commands_ToggleCommand)
- [itembreakwarning](#net_forthecrown_commands_ToggleCommand)
- [npc_dialogue](#net_forthecrown_commands_CommandNpcDialogue)
- [disposal](#net_forthecrown_commands_CommandSelfOrUser)
- [toggleemotes](#net_forthecrown_commands_ToggleCommand)
- [eavesdrop_signs](#net_forthecrown_commands_ToggleCommand)
- [ignoreac](#net_forthecrown_commands_ToggleCommand)
- [mail](#net_forthecrown_commands_CommandMail)
- [stonecutter](#net_forthecrown_commands_ToolBlockCommands)
- [settings](#net_forthecrown_commands_CommandSettings)
- [playtimetop](#net_forthecrown_commands_UserMapTopCommand)
- [feed](#net_forthecrown_commands_CommandSelfOrUser)
- [repair](#net_forthecrown_commands_CommandSelfOrUser)
- [guildrankchat](#net_forthecrown_commands_ToggleCommand)
- [challenges](#net_forthecrown_commands_CommandChallenges)
- [cosmetics](#net_forthecrown_commands_CommandCosmetics)
- [flist](#net_forthecrown_commands_CommandList)
- [heal](#net_forthecrown_commands_CommandSelfOrUser)
- [godmode](#net_forthecrown_commands_ToggleCommand)
- [hulksmash](#net_forthecrown_commands_ToggleCommand)
- [say](#net_forthecrown_commands_CommandSay)
- [toggleguildchat](#net_forthecrown_commands_ToggleCommand$4)
- [ignorelist](#net_forthecrown_commands_CommandIgnoreList)
- [tpatoggle](#net_forthecrown_commands_ToggleCommand)
- [crowntop](#net_forthecrown_commands_CommandLeaderboard$1)
- [wild](#net_forthecrown_commands_CommandWild)

# Commands
# /eavesdrop_muted <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles spying on people's muted messages  
  
Permission: `ftc.admin`  
Aliases: `seemuted`, `see_muted`  
## Usages
```yaml
/eavesdrop_muted
# Toggles spying on people's muted messages

/eavesdrop_muted <player>
# Toggles eavesDrop_muted for a <player>
```

# /playtime <a name="net_forthecrown_commands_UserMapCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.playtime`  
## Usages
```yaml
/playtime
# Shows you your Playtime-Hours

/playtime <player>
# Shows you <player>'s Playtime-Hours

/playtime <player> add <amount: number>
# Adds <amount> of Playtime-Hours to <player>

/playtime <player> set <amount: number>
# Sets the Playtime-Hours of <player> to <amount>

/playtime <player> remove <amount: number>
# Removes <amount> from the Playtime-Hours of <player>

/playtime <player> delete
# Deletes the <player>'s Playtime-Hours data
```

# /rank <a name="net_forthecrown_commands_CommandRank"></a>
Allows you to set your rank  
  
Permission: `ftc.commands.rank`  
Aliases: `ranks`  
## Usages
```yaml
/rank
# Opens the rank menu
```

# /near <a name="net_forthecrown_commands_CommandNear"></a>
Shows nearby players  
  
Permission: `ftc.commands.near`  
Aliases: `nearby`  
## Usages
```yaml
/near <radius: number(1..100,000)>
# Shows all players with a <radius>

/near <user> [<radius: number(1..100,000)>]
# Shows all players near to a <user>
# and within an optional [range]
```

# /gemtop <a name="net_forthecrown_commands_UserMapTopCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.gemtop`  
Aliases: `topgems`  
## Usages
```yaml
/gemtop
# Shows you the Gem Top

/gemtop <page> [<page size: number(5..20)>]
# Shows you the Gem Top on <page>
# If [page size] is not set, then it defaults to 10
```

# /profile <a name="net_forthecrown_commands_CommandProfile"></a>
Displays a user's information  
  
Permission: `ftc.commands.profile`  
Aliases: `user`, `playerprofile`, `gameprofile`  
## Usages
```yaml
/profile
# Shows your profile

/profile <player>
# Shows you a <player>'s profile
```

# /cartography <a name="net_forthecrown_commands_ToolBlockCommands"></a>
Opens a cartography table  
  
Permission: `ftc.commands.cartography`  
## Usages
```yaml
/cartography
# Opens a cartography table
```

# /dynmaptoggle <a name="net_forthecrown_commands_ToggleCommand$1"></a>
Toggles others being able to see you on dynmap  
  
Permission: `ftc.default`  
## Usages
```yaml
/dynmaptoggle
# Toggles others being able to see you on dynmap

/dynmaptoggle <player>
# Toggles dynmapHide for a <player>
```

# /playerridingtoggle <a name="net_forthecrown_commands_ToggleCommand$2"></a>
Toggles being able to ride other players  
  
Permission: `ftc.default`  
Aliases: `ridingtoggle`, `playerriding`  
## Usages
```yaml
/playerridingtoggle
# Toggles being able to ride other players

/playerridingtoggle <player>
# Toggles playerRiding for a <player>
```

# /topvoters <a name="net_forthecrown_commands_UserMapTopCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.topvoters`  
Aliases: `votetop`  
## Usages
```yaml
/topvoters
# Shows you the Top voters

/topvoters <page> [<page size: number(5..20)>]
# Shows you the Top voters on <page>
# If [page size] is not set, then it defaults to 10
```

# /nickname <a name="net_forthecrown_commands_CommandNickname"></a>
Sets your nickname  
  
Permission: `ftc.commands.nickname`  
Aliases: `nick`  
## Usages
```yaml
/nickname
# Clears your nickname

/nickname -clear
# Clears your nickname

/nickname <nick>
# Sets your nickname
```

# /ftc_me <a name="net_forthecrown_commands_CommandMe"></a>
I have no idea what the point of this command is -Julie  
  
Permission: `ftc.default`  
Aliases: `me`  
## Usages
```yaml
/ftc_me <action: string>
# Broadcasts the <action> in chat
# Lets you trick people into thinking you died
# by doing '/me was blown up by Creeper'
```

# /enderchest <a name="net_forthecrown_commands_ToolBlockCommands"></a>
Opens your Ender Chest  
  
Permission: `ftc.commands.enderchest`  
Aliases: `ec`, `echest`  
## Usages
```yaml
/enderchest
# Opens your Ender Chest
```

# /fly <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles flying  
  
Permission: `ftc.admin`  
## Usages
```yaml
/fly
# Toggles flying

/fly <player>
# Toggles flying for a <player>
```

# /votes <a name="net_forthecrown_commands_UserMapCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.votes`  
## Usages
```yaml
/votes
# Shows you your Votes

/votes <player>
# Shows you <player>'s Votes

/votes <player> add <amount: number>
# Adds <amount> of Votes to <player>

/votes <player> set <amount: number>
# Sets the Votes of <player> to <amount>

/votes <player> remove <amount: number>
# Removes <amount> from the Votes of <player>

/votes <player> delete
# Deletes the <player>'s Votes data
```

# /marriagechattoggle <a name="net_forthecrown_commands_ToggleCommand$3"></a>
Toggles all your messages going to marriage chat  
  
Permission: `ftc.marry`  
Aliases: `mchattoggle`, `mct`, `mctoggle`  
## Usages
```yaml
/marriagechattoggle
# Toggles all your messages going to marriage chat

/marriagechattoggle <player>
# Toggles marriageChatToggle for a <player>
```

# /deathtop <a name="net_forthecrown_commands_CommandLeaderboard"></a>
Shows you an objective's leaderboard on the side of your screen  
  
Permission: `ftc.default`  

# /loom <a name="net_forthecrown_commands_ToolBlockCommands"></a>
Opens the loom inventory  
  
Permission: `ftc.commands.loom`  
## Usages
```yaml
/loom
# Opens the loom inventory
```

# /kittycannon <a name="net_forthecrown_commands_CommandDumbThing"></a>
Shoots a kitten at people  
  
Permission: `ftc.commands.kittycannon`  
## Usages
```yaml
/kittycannon
# Shoots a kitten at people
```

# /leave <a name="net_forthecrown_commands_CommandLeave"></a>
I'm out :D  
  
Permission: `ftc.default`  
Aliases: `exit`  

# /hat <a name="net_forthecrown_commands_CommandHat"></a>
Places the item in your hand on your head  
  
Permission: `ftc.commands.hat`  
## Usages
```yaml
/hat
# Places the item in your hand on your head
```

# /workbench <a name="net_forthecrown_commands_ToolBlockCommands"></a>
Opens a workbench  
  
Permission: `ftc.commands.workbench`  
Aliases: `wb`, `craftingtable`  
## Usages
```yaml
/workbench
# Opens a workbench
```

# /reply <a name="net_forthecrown_commands_CommandReply"></a>
Send a message to the last person to send you a message  
  
Permission: `ftc.commands.message`  
Aliases: `er`, `ereply`, `respond`, `r`  
## Usages
```yaml
/reply <message>
# Sends a <message> to the last person that
# messaged you / you messaged.
```

# /guildtop <a name="net_forthecrown_commands_UserMapTopCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.guildtop`  
Aliases: `topguilds`, `gtop`  
## Usages
```yaml
/guildtop
# Shows you the Top by Guild Exp

/guildtop <page> [<page size: number(5..20)>]
# Shows you the Top by Guild Exp on <page>
# If [page size] is not set, then it defaults to 10
```

# /grindstone <a name="net_forthecrown_commands_ToolBlockCommands"></a>
Opens the grindstone menu  
  
Permission: `ftc.commands.grindstone`  
## Usages
```yaml
/grindstone
# Opens the grindstone menu
```

# /paytoggle <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles being able to pay and be payed  
  
Permission: `ftc.commands.pay.toggle`  
## Usages
```yaml
/paytoggle
# Toggles being able to pay and be payed

/paytoggle <player>
# Toggles paying for a <player>
```

# /marrytoggle <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles being able to marry and have people send you proposals  
  
Permission: `ftc.marry`  
Aliases: `togglemarry`  
## Usages
```yaml
/marrytoggle
# Toggles being able to marry and have people send you proposals

/marrytoggle <player>
# Toggles acceptingProposals for a <player>
```

# /profiletoggle <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles your profile being private or public  
  
Permission: `ftc.commands.profile`  
Aliases: `profileprivate`, `profilepublic`  
## Usages
```yaml
/profiletoggle
# Toggles your profile being private or public

/profiletoggle <player>
# Toggles profilePrivate for a <player>
```

# /tell <a name="net_forthecrown_commands_CommandTell"></a>
Sends a message to a player  
  
Permission: `ftc.commands.message`  
Aliases: `emsg`, `tell`, `whisper`, `w`, `msg`, `etell`, `ewhisper`, `pm`, `dm`, `t`, `message`  
## Usages
```yaml
/tell <player> <message>
# Sends a <message> to <player>
# Donators can use color codes and emotes
```

# /toggleinvites <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles being able to invite and be invited to regions  
  
Permission: `ftc.waypoints`  
Aliases: `allowinvites`, `denyinvites`  
## Usages
```yaml
/toggleinvites
# Toggles being able to invite and be invited to regions

/toggleinvites <player>
# Toggles regionInvites for a <player>
```

# /back <a name="net_forthecrown_commands_CommandBack"></a>
Teleports you to your previous location  
  
Permission: `ftc.commands.back`  
Aliases: `return`  
## Usages
```yaml
/back
# Teleports you to your previous location
```

# /rankchat <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles seeing ranks in chat  
  
Permission: `ftc.default`  
Aliases: `chatranks`  
## Usages
```yaml
/rankchat
# Toggles seeing ranks in chat

/rankchat <player>
# Toggles rankedNameTags for a <player>
```

# /smithingtable <a name="net_forthecrown_commands_ToolBlockCommands"></a>
Opens the smithing table  
  
Permission: `ftc.commands.smithingtable`  
Aliases: `smithing`  
## Usages
```yaml
/smithingtable
# Opens the smithing table
```

# /eavesdrop_dm <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles spying on people's DMs  
  
Permission: `ftc.admin`  
Aliases: `seedms`, `see_dms`  
## Usages
```yaml
/eavesdrop_dm
# Toggles spying on people's DMs

/eavesdrop_dm <player>
# Toggles eavesDrop_dm for a <player>
```

# /ignore <a name="net_forthecrown_commands_CommandIgnore"></a>
Makes you ignore/unignore another player  
  
Permission: `ftc.commands.ignore`  
Aliases: `ignoreplayer`, `unignore`, `unignoreplayer`, `block`, `unblock`  
## Usages
```yaml
/ignore <user>
# Ignores/unignores a <user>
```

# /eavesdrop_mchat <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles seeing what people say in marriage dms  
  
Permission: `ftc.admin`  
Aliases: `seemchat`, `seemarriage`, `see_mchat`, `see_marriage`  
## Usages
```yaml
/eavesdrop_mchat
# Toggles seeing what people say in marriage dms

/eavesdrop_mchat <player>
# Toggles eavesDrop_mChat for a <player>
```

# /afk <a name="net_forthecrown_commands_CommandAfk"></a>
Marks or un-marks you as AFK  
  
Permission: `ftc.default`  
Aliases: `away`  
## Usages
```yaml
/afk
# Sets you afk/unafk

/afk <message>
# AFKs you with an AFK message
```

# /baltop <a name="net_forthecrown_commands_UserMapTopCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.baltop`  
Aliases: `balancetop`, `banktop`, `topbals`, `topbalances`  
## Usages
```yaml
/baltop
# Shows you the Top balances

/baltop <page> [<page size: number(5..20)>]
# Shows you the Top balances on <page>
# If [page size] is not set, then it defaults to 10
```

# /balance <a name="net_forthecrown_commands_UserMapCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.balance`  
Aliases: `bal`, `bank`, `cash`, `money`, `ebal`  
## Usages
```yaml
/balance
# Shows you your Rhines

/balance <player>
# Shows you <player>'s Rhines

/balance <player> add <amount: number>
# Adds <amount> of Rhines to <player>

/balance <player> set <amount: number>
# Sets the Rhines of <player> to <amount>

/balance <player> remove <amount: number>
# Removes <amount> from the Rhines of <player>

/balance <player> delete
# Deletes the <player>'s Rhines data
```

# /beezooka <a name="net_forthecrown_commands_CommandDumbThing"></a>
Shoots a bee :D  
  
Permission: `ftc.commands.beezooka`  
## Usages
```yaml
/beezooka
# Shoots a bee :D
```

# /suicide <a name="net_forthecrown_commands_CommandSuicide"></a>
Commits suicide D:  
  
Permission: `ftc.commands.suicide`  
## Usages
```yaml
/suicide
# Commits suicide D:
```

# /setspawn <a name="net_forthecrown_commands_CommandSetSpawn"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
## Usages
```yaml
/setspawn world
# Sets the world's spawn to where you are

/setspawn world <pos: x,y,z>
# Sets the world's spawn to <pos>

/setspawn server
# Sets the server's spawn to where you are

/setspawn server <pos: x,y,z>
# Sets the server's spawn to <pos>
```

# /gems <a name="net_forthecrown_commands_UserMapCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.gems`  
## Usages
```yaml
/gems
# Shows you your Gems

/gems <player>
# Shows you <player>'s Gems

/gems <player> add <amount: number>
# Adds <amount> of Gems to <player>

/gems <player> set <amount: number>
# Sets the Gems of <player> to <amount>

/gems <player> remove <amount: number>
# Removes <amount> from the Gems of <player>

/gems <player> delete
# Deletes the <player>'s Gems data
```

# /staffchattoggle <a name="net_forthecrown_commands_CommandSelfOrUser"></a>
Toggles all chat messages going to staff chat  
  
Permission: `ftc.staffchat`  
Aliases: `sct`, `sctoggle`  
## Usages
```yaml
/staffchattoggle
# Toggles all chat messages going to staff chat for yourself

/staffchattoggle <player>
# Toggles all chat messages going to staff chat for a <player>
```

# /eavesdrop_gchat <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles seeing guild chats  
  
Permission: `ftc.admin`  
## Usages
```yaml
/eavesdrop_gchat
# Toggles seeing guild chats

/eavesdrop_gchat <player>
# Toggles eavesDrop_guildChat for a <player>
```

# /itembreakwarning <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles seeing item breaking warnings  
  
Permission: `ftc.default`  
Aliases: `itemdurability`, `durabilitywarnings`  
## Usages
```yaml
/itembreakwarning
# Toggles seeing item breaking warnings

/itembreakwarning <player>
# Toggles durabilityAlerts for a <player>
```

# /npc_dialogue <a name="net_forthecrown_commands_CommandNpcDialogue"></a>
Secret command... so sush!  
  
Permission: `ftc.default`  

# /disposal <a name="net_forthecrown_commands_CommandSelfOrUser"></a>
Opens a menu to dispose of items for yourself or another player  
  
Permission: `ftc.commands.disposal`  
Aliases: `bin`  
## Usages
```yaml
/disposal
# Opens a menu to dispose of items for yourself

/disposal <player>
# Opens a menu to dispose of items for a <player>
```

# /toggleemotes <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles being able to emote to people and for people to emote at you  
  
Permission: `ftc.emotes`  
Aliases: `emotetoggle`  
## Usages
```yaml
/toggleemotes
# Toggles being able to emote to people and for people to emote at you

/toggleemotes <player>
# Toggles emotes for a <player>
```

# /eavesdrop_signs <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles seeing what people write on signs  
  
Permission: `ftc.admin`  
Aliases: `seesigns`, `see_signs`  
## Usages
```yaml
/eavesdrop_signs
# Toggles seeing what people write on signs

/eavesdrop_signs <player>
# Toggles eavesDrop_signs for a <player>
```

# /ignoreac <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles seeing automated server announcements  
  
Permission: `ftc.commands.ignoreac`  
Aliases: `ignorebroadcasts`, `ignorebc`, `ignoreannouncements`  
## Usages
```yaml
/ignoreac
# Toggles seeing automated server announcements

/ignoreac <player>
# Toggles ignoringBroadcasts for a <player>
```

# /mail <a name="net_forthecrown_commands_CommandMail"></a>
Lets you send, read and claim items from mail  
  
Permission: `ftc.mail`  
## Usages
```yaml
/mail [<page>] [<page size: number(5..20)>]
# Shows you your mail, page and page
# size are optional arguments

/mail send <user> <message>
# Sends a <user> a <message>

/mail send_item <user> <message>
# Sends a <user> a <message> and then
# opens a menu to send an item with the mail

/mail clear
# Clears all your mail
# messages that have unclaimed items
# will not cleared

/mail claim <index: number>
# Claims the mail at the given index
# This will mostly not be needed, as
# the [claim] button will do this for you

/mail read_other <user> [<page>] [<page size: number(5..20)>]
# Reads a user's mail

/mail clear <user>
# Clears ALL of the user's mail, even unclaimed mail

/mail send -all <message>
# Sends a <message> to ALL users, even offline

/mail send_item -all <message>
# Sends a <message> with an item to
# ALL users, even offline

/mail send_admin [users | -all] message=<message> [item=<item>] [rhines=<amount>] [gems=<gems>] [tag=<tag>] [script=<claim script>]
# Sends a message to either all users or a specific user
# with the given parameters
```

# /stonecutter <a name="net_forthecrown_commands_ToolBlockCommands"></a>
Opens the stone cutter menu  
  
Permission: `ftc.commands.stonecutter`  
## Usages
```yaml
/stonecutter
# Opens the stone cutter menu
```

# /settings <a name="net_forthecrown_commands_CommandSettings"></a>
Opens the settings book  
  
Permission: `ftc.commands.settings`  
Aliases: `options`  
## Usages
```yaml
/settings
# Opens the settings book
```

# /playtimetop <a name="net_forthecrown_commands_UserMapTopCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.commands.playtimetop`  
Aliases: `nolifetop`, `topplayers`  
## Usages
```yaml
/playtimetop
# Shows you the Top by playtime

/playtimetop <page> [<page size: number(5..20)>]
# Shows you the Top by playtime on <page>
# If [page size] is not set, then it defaults to 10
```

# /feed <a name="net_forthecrown_commands_CommandSelfOrUser"></a>
Feeds yourself or a player  
  
Permission: `ftc.commands.feed`  
## Usages
```yaml
/feed
# Feeds yourself

/feed <player>
# Feeds a <player>
```

# /repair <a name="net_forthecrown_commands_CommandSelfOrUser"></a>
Repairs the item you're holding  
  
Permission: `ftc.commands.repair`  
## Usages
```yaml
/repair
# Repairs an item held by yourself

/repair <player>
# Repairs an item held by a <player>
```

# /guildrankchat <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles seeing ranks in guild chat  
  
Permission: `ftc.guild`  
Aliases: `gcranks`, `gchatranks`  
## Usages
```yaml
/guildrankchat
# Toggles seeing ranks in guild chat

/guildrankchat <player>
# Toggles guildRankedNameTags for a <player>
```

# /challenges <a name="net_forthecrown_commands_CommandChallenges"></a>
Opens the challenge book  
  
Permission: `ftc.challenges`  
## Usages
```yaml
/challenges
# Opens the challenge book

/challenges list
# Lists all loaded challenges

/challenges list_active
# Lists all active challenges

/challenges give_points <challenge> <player> [<points: number(1..)>]
# Gives [points] for a <challenge> to a <player>
# If [points] is not set, defaults to 1

/challenges trigger <challenge> <player>
# Triggers a <challenge> for a <player>
# What 'triggering' means, varies based on implementation

/challenges complete_all <category> <user>
# Completes all active challenges in a <category> for a
# <user>

/challenges reset [<category>]
# Resets all challenges in a [category]. If a [category] is
# not set, it resets all categories

/challenges items <challenge> set_active [<item>]
# Sets an [item] to be a <challenge>'s active item
# If [item] is not set, then your held item is used

/challenges items <challenge> reroll
# Forces a <challenge> to re-roll it's chosen item

/challenges items <challenge> chests
# Lists all chests a <challenge> is getting items from
# Note:
# Chests are the 'item sources' from which item challenges
# pick their items at random. These chests have to exist in
# in the actual world

/challenges items <challenge> chests add [<block: x,y,z>]
# Adds a chest item source to a <challenge>
# If <block> is not set, the block you are looking at
# is used instead

/challenges items <challenge> chests remove <index>
# Removes a chest item source from a <challenge> at <index>
# To find the <index> do /challenges items <challenge> chests

/challenges items <challenge> chests clear
# Clears all chest item sources from a <challenge>
```

# /cosmetics <a name="net_forthecrown_commands_CommandCosmetics"></a>
Opens the cosmetics menu  
  
Permission: `ftc.default`  
## Usages
```yaml
/cosmetics
# Opens the cosmetics menu
```

# /flist <a name="net_forthecrown_commands_CommandList"></a>
Lists all players on the server  
  
Permission: `ftc.commands.list`  
Aliases: `list`, `elist`, `playerlist`  

# /heal <a name="net_forthecrown_commands_CommandSelfOrUser"></a>
Heals yourself or another player  
  
Permission: `ftc.commands.heal`  
## Usages
```yaml
/heal
# Heals yourself

/heal <player>
# Heals a <player>
```

# /godmode <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles god mode  
  
Permission: `ftc.admin`  
Aliases: `god`, `togglegod`, `togglegodmode`  
## Usages
```yaml
/godmode
# Toggles god mode

/godmode <player>
# Toggles godMode for a <player>
```

# /hulksmash <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles whether you quickly teleport to poles or hulk smash onto them  
  
Permission: `ftc.waypoints`  
Aliases: `togglehulk`, `togglehulksmash`  
## Usages
```yaml
/hulksmash
# Toggles whether you quickly teleport to poles or hulk smash onto them

/hulksmash <player>
# Toggles hulkSmashing for a <player>
```

# /say <a name="net_forthecrown_commands_CommandSay"></a>
Says a message in chat  
  
Permission: `ftc.default`  

# /toggleguildchat <a name="net_forthecrown_commands_ToggleCommand$4"></a>
Toggles all chat messages being sent to /gc  
  
Permission: `ftc.guild`  
Aliases: `gct`, `gctoggle`  
## Usages
```yaml
/toggleguildchat
# Toggles all chat messages being sent to /gc

/toggleguildchat <player>
# Toggles guildChatToggled for a <player>
```

# /ignorelist <a name="net_forthecrown_commands_CommandIgnoreList"></a>
Displays all the ignored players  
  
Permission: `ftc.commands.ignore`  
Aliases: `blocked`, `blockedplayers`, `blockedlist`, `ignoring`, `ignored`, `ignores`, `ignoredlist`, `ignoredplayers`, `listignores`, `listignored`  
## Usages
```yaml
/ignorelist
# Shows your ignored players

/ignorelist <player>
# Shows a <player>'s ignored players
```

# /tpatoggle <a name="net_forthecrown_commands_ToggleCommand"></a>
Toggles being able to tpa to people  
  
Permission: `ftc.commands.tpa`  
Aliases: `toggletpa`  
## Usages
```yaml
/tpatoggle
# Toggles being able to tpa to people

/tpatoggle <player>
# Toggles tpa for a <player>
```

# /crowntop <a name="net_forthecrown_commands_CommandLeaderboard$1"></a>
Shows you an objective's leaderboard on the side of your screen  
  
Permission: `ftc.default`  

# /wild <a name="net_forthecrown_commands_CommandWild"></a>
Puts you in the wild, only available in the Resource World  
  
Permission: `ftc.default`  
## Usages
```yaml
/wild
# Teleports you into the wilderness.
# This command only works at spawn or
# in the Resource World

/wild <entities> [<world>]
# Teleports a <player> into the wilderness
# in a [world]. If [world] is not set, then
# the <entities> is teleported in their own world
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Tue Mar 21 15:10:51 EET 2023`  
Plugin version: `1.19.4-1719-SNAPSHOT`  
Total commands: 70