---
title: "Markets"
linkTitle: "Markets"
type: docs
weight: 1
description: >
  Markets Commands
---

# Table of Contents
- [/market](#commands_markets_CommandMarket)
- [/marketappeal](#commands_markets_CommandMarketAppeal)
- [/marketediting](#commands_markets_CommandMarketEditing)
- [/marketevict](#commands_markets_CommandMarketWarning)
- [/mergeshop](#commands_markets_CommandMergeShop)
- [/shoptrust](#commands_markets_CommandShopTrust)
- [/transfershop](#commands_markets_CommandTransferShop)
- [/unclaimshop](#commands_markets_CommandUnclaimShop)
- [/unmerge](#commands_markets_CommandUnmerge)

# Commands
## /market <a name="commands_markets_CommandMarket"></a>
General purpose commands to manage markets  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `markets`, `shops`  
### Usages
```yaml
/market refresh_all
# Refreshes all existing shops
# This will just ensure every shop's entrance
# exists and is displaying the correct info

/market create <region name>
# Creates a new shop, linked to <region name>.
# Every shop has to be linked to a world guard
# region for membership and protection

/market list
# Lists all existing markets

/market <shop name>
# Lists info about the <shop>

/market <shop name> claim <user>
# Claims the <shop> for the <user>.
# Only works if the shop is not already claimed

/market <shop name> connections <other shop> <add | remove>
# Adds/removes a 'connection' with another
# shop. Connections allow shops to be merged

/market <shop name> delete
# Deletes the shop

/market <shop name> entrances add
# Adds a shop entrance, with the notice set
# as your position, the sign position as the
# block above you and the direction being the
# direction you're facing

/market <shop name> entrances add <notice: x,y,z> <sign: x,y,z> [<direction>]
# Adds a shop entrance with the given parameters
# If [direction] is not set, uses your direction

/market <shop name> entrances remove <index>
# Removes the entrance with the given index

/market <shop name> entrances merge <other shop>
# Merges <shop name> with <other shop>

/market <shop name> unmerge
# Unmerges the shop

/market <shop name> price <price: number(-1..)>
# Sets the shop's price, 0 means free
# If the price is -1, then the shop will use
# a default price set in the markets config

/market <shop name> wg_region
# Displays info about the <shop>'s world guard region

/market <shop name> unclaim
# Unclaims the shop, just removes the owner

/market <shop name> unclaim_complete
# Unclaims the shop, removes the owner and then
# resets the shop

/market <shop name> reset
# Resets the shop
```

## /marketappeal <a name="commands_markets_CommandMarketAppeal"></a>
Appeals an automated market eviction  
  
**Command metadata**:  
Permission: `ftc.markets`  
### Usages
```yaml
/marketappeal
# Appeals an automated market eviction
```

## /marketediting <a name="commands_markets_CommandMarketEditing"></a>
Allows/disallows shop members to edit sign shops in your shop  
  
**Command metadata**:  
Permission: `ftc.markets`  
Aliases: `toggleshopediting`, `togglemarketediting`  
### Usages
```yaml
/marketediting
# Allows/disallows shop members to edit sign shops in your shop
```

## /marketevict <a name="commands_markets_CommandMarketWarning"></a>
Issues/revokes a shop eviction  
  
**Command metadata**:  
Permission: `ftc.markets.warning`  
Aliases: `shopevict`, `evictshop`, `evictmarket`  
### Usages
```yaml
/marketevict <user | shop> <value> <time> <reason>
# Starts a market eviction with <reason>.
# The owner will be evicted after <time> has passed

/marketevict <user | shop> <value> undo
# Cancels a shop eviction
```

## /mergeshop <a name="commands_markets_CommandMergeShop"></a>
Request to merge your shop with someone else's  
  
**Command metadata**:  
Permission: `ftc.markets`  
Aliases: `mergemarket`, `shopmerge`, `marketmerge`  
### Usages
```yaml
/mergeshop <user>
# Requests to merge your shop with a <user>'s shop

/mergeshop <user> confirm
# Confirms a merge request that came from a <user>

/mergeshop <user> deny
# Denies a merge request that came from a <user>

/mergeshop <user> cancel
# Cancels a merge request sent to a <user>
```

## /shoptrust <a name="commands_markets_CommandShopTrust"></a>
Trusts/untrusts a player in your shop  
  
**Command metadata**:  
Permission: `ftc.markets`  
Aliases: `shopuntrust`, `markettrust`, `marketuntrust`  
### Usages
```yaml
/shoptrust <user>
# Trusts/untrusts a <user>
```

## /transfershop <a name="commands_markets_CommandTransferShop"></a>
Transfers a player's shop in Hazelguard to another player  
  
**Command metadata**:  
Permission: `ftc.markets`  
Aliases: `transfermarket`, `shoptransfer`, `markettransfer`  
### Usages
```yaml
/transfershop <user>
# Transfers the shop you own to a <user>
```

## /unclaimshop <a name="commands_markets_CommandUnclaimShop"></a>
Makes you unclaim your shop in Hazelguard  
  
**Command metadata**:  
Permission: `ftc.markets`  
Aliases: `unclaimmarket`  
### Usages
```yaml
/unclaimshop
# Makes you unclaim your shop in Hazelguard
```

## /unmerge <a name="commands_markets_CommandUnmerge"></a>
Unmerges the shop you own with the shop it's merged with  
  
**Command metadata**:  
Permission: `ftc.markets`  
Aliases: `marketunmerge`, `shopunmerge`, `unmergeshop`, `unmergemarket`  
### Usages
```yaml
/unmerge
# Unmerges the shop you own with the shop it's merged with
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Thu Mar 30 22:08:46 CEST 2023`  
Plugin version: `1.19.4-1733-RELEASE`  
Total commands: 9