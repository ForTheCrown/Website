---
title: "User"
linkTitle: "User"
type: docs
weight: 1
description: >
  User Commands
---

# Table of Contents
- [user_titles](#net_forthecrown_commands_user_UserTitlesNode)
- [user_earnings](#net_forthecrown_commands_user_UserEarningsNode)
- [user_timestamps](#net_forthecrown_commands_user_UserTimeNode)
- [user_tab](#net_forthecrown_commands_user_UserTabNode)
- [user_cosmetics](#net_forthecrown_commands_user_UserCosmeticsNode)
- [user_alts](#net_forthecrown_commands_user_UserAltNode)
- [ftcuser](#net_forthecrown_commands_user_UserCommands$UserCommand)

# Commands
# /user_titles <a name="net_forthecrown_commands_user_UserTitlesNode"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
## Usages
```yaml
/user_titles <user>
# Displays a user's active title,
# available titles and tier

/user_titles <user> tier
# Shows a user's tier

/user_titles <user> tier <tier>
# Sets the user's tiers

/user_titles <user> title
# Show's a user's active title

/user_titles <user> title <title>
# Sets a user's active title

/user_titles <user> available_titles
# Lists a user's available titles

/user_titles <user> available_titles add <title list>
# Adds all titles to a user

/user_titles <user> available_titles remove <title list>
# Removes all titles from a user
```

# /user_earnings <a name="net_forthecrown_commands_user_UserEarningsNode"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
Aliases: `userearnings`  
## Usages
```yaml
/user_earnings <user> auto_sell
# Lists a user's auto sell materials

/user_earnings <user> auto_sell clear
# Clears a user's auto sell materials list

/user_earnings <user> auto_sell add <material>
# Adds a material to a user's auto sell list

/user_earnings <user> auto_sell remove <material>
# Removes a material from a user's auto sell list

/user_earnings <user> earned
# Lists how many Rhines a user has earned
# from every material they've sold

/user_earnings <user> earned clear
# Clears all the user's earnings data

/user_earnings <user> earned set <material> <amount: number>
# Sets the <amount> the user has earned
# from the <material>

/user_earnings <user> earned add <material> <amount: number(1..)>
# Adds <amount> to the earned amount

/user_earnings <user> earned remove <material> <amount: number(1..)>
# Removes <amount> from the earnings of
# <material>
```

# /user_timestamps <a name="net_forthecrown_commands_user_UserTimeNode"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
## Usages
```yaml
/user_timestamps <user>
# Shows a user's time fields as
# human-readable dates

/user_timestamps <user> set <time field> <time stamp: number>
# Sets the <time field> to the given <time stamp>
# value, the <time stamp> is a UNIX millisecond
# time stamp

/user_timestamps <user> set <time field> -now
# Sets the <time field> to the current
# moment in time.

/user_timestamps <user> unset <time field>
# Resets the <time field> for a user
```

# /user_tab <a name="net_forthecrown_commands_user_UserTabNode"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
## Usages
```yaml
/user_tab <user> <prefix | suffix | tabName>
# Shows the current value

/user_tab <user> <prefix | suffix | tabName> -clears
# Clears the value

/user_tab <user> <prefix | suffix | tabName> <text>
# Sets the value
```

# /user_cosmetics <a name="net_forthecrown_commands_user_UserCosmeticsNode"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
Aliases: `user_effects`, `usercosmetics`, `usereffects`  
## Usages
```yaml
/user_cosmetics <user> <effect type>
# Shows a user's active and available <effect types>

/user_cosmetics <user> <effect type> set <cosmetic>
# Sets the user's active <effect type>

/user_cosmetics <user> <effect type> unset
# Clears the user's active <effect type> cosmetic

/user_cosmetics <user> <effect type> clear
# Clears the user's available
# <effect type> cosmetics

/user_cosmetics <user> <effect type> add <cosmetic>
# Adds the <cosmetic> to the user's
# cosmetic effect list

/user_cosmetics <user> <effect type> remove <cosmetic>
# Removes the <cosmetic> from the user's
# available cosmetics list
```

# /user_alts <a name="net_forthecrown_commands_user_UserAltNode"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
## Usages
```yaml
/user_alts <user>
# Lists a <user>'s alt accounts and main account,
# if they have them

/user_alts <user> add <alt>
# Adds a <target> as an alt for a <user>

/user_alts <user> remove <alt>
# Removes a <target> as an alt for a <user>

/user_alts <user> clear
# Clears all alt accounts that belong to a <user>
```

# /ftcuser <a name="net_forthecrown_commands_user_UserCommands$UserCommand"></a>
An FTC command (default description)  
  
Permission: `ftc.admin`  
Aliases: `users`, `user`  
## Usages
```yaml
/ftcuser <user> timestamps
# Shows a user's time fields as
# human-readable dates

/ftcuser <user> timestamps set <time field> <time stamp: number>
# Sets the <time field> to the given <time stamp>
# value, the <time stamp> is a UNIX millisecond
# time stamp

/ftcuser <user> timestamps set <time field> -now
# Sets the <time field> to the current
# moment in time.

/ftcuser <user> timestamps unset <time field>
# Resets the <time field> for a user

/ftcuser <user> titles
# Displays a user's active title,
# available titles and tier

/ftcuser <user> titles tier
# Shows a user's tier

/ftcuser <user> titles tier <tier>
# Sets the user's tiers

/ftcuser <user> titles title
# Show's a user's active title

/ftcuser <user> titles title <title>
# Sets a user's active title

/ftcuser <user> titles available_titles
# Lists a user's available titles

/ftcuser <user> titles available_titles add <title list>
# Adds all titles to a user

/ftcuser <user> titles available_titles remove <title list>
# Removes all titles from a user

/ftcuser <user> cosmetics <effect type>
# Shows a user's active and available <effect types>

/ftcuser <user> cosmetics <effect type> set <cosmetic>
# Sets the user's active <effect type>

/ftcuser <user> cosmetics <effect type> unset
# Clears the user's active <effect type> cosmetic

/ftcuser <user> cosmetics <effect type> clear
# Clears the user's available
# <effect type> cosmetics

/ftcuser <user> cosmetics <effect type> add <cosmetic>
# Adds the <cosmetic> to the user's
# cosmetic effect list

/ftcuser <user> cosmetics <effect type> remove <cosmetic>
# Removes the <cosmetic> from the user's
# available cosmetics list

/ftcuser <user> earnings auto_sell
# Lists a user's auto sell materials

/ftcuser <user> earnings auto_sell clear
# Clears a user's auto sell materials list

/ftcuser <user> earnings auto_sell add <material>
# Adds a material to a user's auto sell list

/ftcuser <user> earnings auto_sell remove <material>
# Removes a material from a user's auto sell list

/ftcuser <user> earnings earned
# Lists how many Rhines a user has earned
# from every material they've sold

/ftcuser <user> earnings earned clear
# Clears all the user's earnings data

/ftcuser <user> earnings earned set <material> <amount: number>
# Sets the <amount> the user has earned
# from the <material>

/ftcuser <user> earnings earned add <material> <amount: number(1..)>
# Adds <amount> to the earned amount

/ftcuser <user> earnings earned remove <material> <amount: number(1..)>
# Removes <amount> from the earnings of
# <material>

/ftcuser <user> tab <prefix | suffix | tabName>
# Shows the current value

/ftcuser <user> tab <prefix | suffix | tabName> -clears
# Clears the value

/ftcuser <user> tab <prefix | suffix | tabName> <text>
# Sets the value

/ftcuser <user> alts
# Lists a <user>'s alt accounts and main account,
# if they have them

/ftcuser <user> alts add <alt>
# Adds a <target> as an alt for a <user>

/ftcuser <user> alts remove <alt>
# Removes a <target> as an alt for a <user>

/ftcuser <user> alts clear
# Clears all alt accounts that belong to a <user>
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Tue Mar 21 15:10:51 EET 2023`  
Plugin version: `1.19.4-1719-SNAPSHOT`  
Total commands: 7