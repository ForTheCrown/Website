---
title: "economy/market"
linkTitle: "economy/market"
type: docs
weight: 1
description: >
  economy/market commands
---


## /market
General purpose commands to manage markets  
  
**Permission**: `ftc.markets.admin`  
**Aliases**: `markets`, `shops`  
**Uses**:
- <pre class="command-usage-arguments">/market refresh_all</pre>  
  Refreshes all existing shops  
  This will just ensure every shop's entrance  
  exists and is displaying the correct info  
- <pre class="command-usage-arguments">/market create &lt;region name&gt;</pre>  
  Creates a new shop, linked to region name.  
  Every shop has to be linked to a world guard  
  region for membership and protection  
- <pre class="command-usage-arguments">/market list</pre>  
  Lists all existing markets  
- <pre class="command-usage-arguments">/market &lt;shop name&gt;</pre>  
  Lists info about the shop  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; claim &lt;user&gt;</pre>  
  Claims the shop for the user.  
  Only works if the shop is not already claimed  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; connections &lt;other shop&gt; &lt;add | remove&gt;</pre>  
  Adds/removes a 'connection' with another  
  shop. Connections allow shops to be merged  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; delete</pre>  
  Deletes the shop  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; entrances add</pre>  
  Adds a shop entrance, with the notice set  
  as your position, the sign position as the  
  block above you and the direction being the  
  direction you're facing  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; entrances add &lt;notice: x,y,z&gt; &lt;sign: x,y,z&gt; [&lt;direction&gt;]</pre>  
  Adds a shop entrance with the given parameters  
  If [direction] is not set, uses your direction  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; entrances remove &lt;index&gt;</pre>  
  Removes the entrance with the given index  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; entrances merge &lt;other shop&gt;</pre>  
  Merges shop name with other shop  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; unmerge</pre>  
  Unmerges the shop  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; price &lt;price: number(-1..)&gt;</pre>  
  Sets the shop's price, 0 means free  
  If the price is -1, then the shop will use  
  a default price set in the markets config  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; wg_region</pre>  
  Displays info about the shop's world guard region  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; unclaim</pre>  
  Unclaims the shop, just removes the owner  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; unclaim_complete</pre>  
  Unclaims the shop, removes the owner and then  
  resets the shop  
- <pre class="command-usage-arguments">/market &lt;shop name&gt; reset</pre>  
  Resets the shop  

## /marketappeal
Appeals an automated market eviction  
  
**Permission**: `ftc.markets`  
**Uses**:
- <pre class="command-usage-arguments">/marketappeal</pre>  
  Appeals an automated market eviction  

## /marketediting
Allows/disallows shop members to edit sign shops in your shop  
  
**Permission**: `ftc.markets`  
**Aliases**: `toggleshopediting`, `togglemarketediting`  
**Uses**:
- <pre class="command-usage-arguments">/marketediting</pre>  
  Allows/disallows shop members to edit sign shops in your shop  

## /marketevict
Issues/revokes a shop eviction  
  
**Permission**: `ftc.markets.admin`  
**Aliases**: `shopevict`, `evictshop`, `evictmarket`  
**Uses**:
- <pre class="command-usage-arguments">/marketevict &lt;user | shop&gt; &lt;value&gt; &lt;time&gt; &lt;reason&gt;</pre>  
  Starts a market eviction with reason.  
  The owner will be evicted after time has passed  
- <pre class="command-usage-arguments">/marketevict &lt;user | shop&gt; &lt;value&gt; undo</pre>  
  Cancels a shop eviction  

## /mergeshop
Request to merge your shop with someone else's  
  
**Permission**: `ftc.markets`  
**Aliases**: `mergemarket`, `shopmerge`, `marketmerge`  
**Uses**:
- <pre class="command-usage-arguments">/mergeshop &lt;user&gt;</pre>  
  Requests to merge your shop with a user's shop  
- <pre class="command-usage-arguments">/mergeshop &lt;user&gt; confirm</pre>  
  Confirms a merge request that came from a user  
- <pre class="command-usage-arguments">/mergeshop &lt;user&gt; deny</pre>  
  Denies a merge request that came from a user  
- <pre class="command-usage-arguments">/mergeshop &lt;user&gt; cancel</pre>  
  Cancels a merge request sent to a user  

## /shoptrust
Trusts/untrusts a player in your shop  
  
**Permission**: `ftc.markets`  
**Aliases**: `shopuntrust`, `markettrust`, `marketuntrust`  
**Uses**:
- <pre class="command-usage-arguments">/shoptrust &lt;user&gt;</pre>  
  Trusts/untrusts a user  

## /transfershop
Transfers a player's shop in Hazelguard to another player  
  
**Permission**: `ftc.markets`  
**Aliases**: `transfermarket`, `shoptransfer`, `markettransfer`  
**Uses**:
- <pre class="command-usage-arguments">/transfershop &lt;user&gt;</pre>  
  Transfers the shop you own to a user  

## /unclaimshop
Makes you unclaim your shop in Hazelguard  
  
**Permission**: `ftc.markets`  
**Aliases**: `unclaimmarket`  
**Uses**:
- <pre class="command-usage-arguments">/unclaimshop</pre>  
  Makes you unclaim your shop in Hazelguard  

## /unmerge
Unmerges the shop you own with the shop it's merged with  
  
**Permission**: `ftc.markets`  
**Aliases**: `marketunmerge`, `shopunmerge`, `unmergeshop`, `unmergemarket`  
**Uses**:
- <pre class="command-usage-arguments">/unmerge</pre>  
  Unmerges the shop you own with the shop it's merged with  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 9