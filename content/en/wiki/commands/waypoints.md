---
title: "waypoints"
linkTitle: "waypoints"
type: docs
weight: 1
description: >
  waypoints commands
---


## /findpole
Shows you the nearest waypoint  
  
**Permission**: `ftc.waypoints`  
**Aliases**: `findpost`, `findwaypoint`  

## /homewaypoint
Takes you to your home waypoint  
  
**Permission**: `ftc.waypoints`  
**Aliases**: `homepole`, `homepost`  
**Uses**:
- <pre class="command-usage-arguments">/homewaypoint</pre>  
  Takes you to your home waypoint  

## /invite
Invites users to your home waypoint  
  
**Permission**: `ftc.waypoints`  
**Uses**:
- <pre class="command-usage-arguments">/invite &lt;users&gt;</pre>  
  Invites users to your home waypoint  

## /listwaypoints
Lists named waypoints  
  
**Permission**: `ftc.waypoints`  
**Aliases**: `listregions`, `regions`, `regionlist`, `waypointlist`  
**Uses**:
- <pre class="command-usage-arguments">/listwaypoints</pre>  
  Lists named waypoints  
- <pre class="command-usage-arguments">/listwaypoints &lt;page: number(1..)&gt; [&lt;page size: number(5..20)&gt;]</pre>  
  Lists named waypoints on a specific page  

## /movein
Sets your home waypoint  
  
**Permission**: `ftc.waypoints`  
**Aliases**: `sethomepole`, `sethomepost`  
**Uses**:
- <pre class="command-usage-arguments">/movein</pre>  
  Sets your home waypoint  

## /spawn
Alias for '/vr Hazelguard'  
  
**Permission**: `ftc.waypoints`  

## /visit
Visits a teleport waypoint  
  
**Permission**: `ftc.waypoints`  
**Aliases**: `v`, `vr`, `visitregion`  
**Uses**:
- <pre class="command-usage-arguments">/visit &lt;waypoint name&gt;</pre>  
  Visits a teleport waypoint  

## /waypointgui
Opens the Waypoint GUI  
  
**Permission**: `ftc.waypoints`  

## /waypoints
Waypoints admin commands  
  
**Permission**: `ftc.waypoints.admin`  
**Uses**:
- <pre class="command-usage-arguments">/waypoints save</pre>  
  Saves all waypoints  
- <pre class="command-usage-arguments">/waypoints reload-config</pre>  
  Reloads the waypoints config  
- <pre class="command-usage-arguments">/waypoints reload-all</pre>  
  Reloads ALL waypoints  
- <pre class="command-usage-arguments">/waypoints update-all</pre>  
  Updates all waypoints  
- <pre class="command-usage-arguments">/waypoints info &lt;waypoint&gt;</pre>  
  Shows info about a waypoint  
- <pre class="command-usage-arguments">/waypoints update &lt;waypoint&gt;</pre>  
  Updates a specific waypoint  
- <pre class="command-usage-arguments">/waypoints remove &lt;waypoint&gt;</pre>  
  Deletes a waypoint  
- <pre class="command-usage-arguments">/waypoints draw-bounds &lt;waypoint&gt;</pre>  
  Draws the bounds of a waypoint  
- <pre class="command-usage-arguments">/waypoints create admin</pre>  
  Creates an invisible admin waypoint  
- <pre class="command-usage-arguments">/waypoints create region-pole</pre>  
  Creates a region-pole waypoint  
- <pre class="command-usage-arguments">/waypoints move &lt;waypoint&gt;</pre>  
  Moves a waypoint to where you're standing  
- <pre class="command-usage-arguments">/waypoints move &lt;waypoint&gt; &lt;pos: x y z&gt;</pre>  
  Moves a waypoint to a specified xyz position  
- <pre class="command-usage-arguments">/waypoints residents list &lt;waypoint&gt;</pre>  
  Lists all residents in a waypoints  
- <pre class="command-usage-arguments">/waypoints residents add &lt;waypoint&gt; &lt;players&gt;</pre>  
  Adds all players to be residents of waypoint  
- <pre class="command-usage-arguments">/waypoints residents remove &lt;waypoint&gt; &lt;resident&gt;</pre>  
  Removes a resident from a waypoint  
- <pre class="command-usage-arguments">/waypoints residents set &lt;waypoint&gt; &lt;player&gt; &lt;time&gt;</pre>  
  Sets a player to be a resident of a waypoint with a specific movein time  
- <pre class="command-usage-arguments">/waypoints residents clear &lt;waypoint&gt;</pre>  
  Removes all residents from a waypoint  
- <pre class="command-usage-arguments">/waypoints property list &lt;waypoint&gt;</pre>  
  Lists all property values in a waypoint  
- <pre class="command-usage-arguments">/waypoints property unset &lt;waypoint&gt; &lt;property&gt;</pre>  
  Removes a property's value from a waypoint  
- <pre class="command-usage-arguments">/waypoints property set &lt;waypoint&gt; &lt;property&gt; &lt;value&gt;</pre>  
  Sets a property's value for a specific waypoint  
- <pre class="command-usage-arguments">/waypoints property get &lt;waypoint&gt; &lt;property&gt;</pre>  
  Gets a property's value  
- <pre class="command-usage-arguments">/waypoints column clear &lt;waypoint&gt;</pre>  
  Breaks the center column of a waypoint  
- <pre class="command-usage-arguments">/waypoints column place &lt;waypoint&gt;</pre>  
  Places the center column of a waypoint  
- <pre class="command-usage-arguments">/waypoints platform place &lt;waypoint&gt;</pre>  
  Places a platform for a waypoint  
- <pre class="command-usage-arguments">/waypoints platform break &lt;waypoint&gt;</pre>  
  Breaks a waypoint's platform  
- <pre class="command-usage-arguments">/waypoints description get &lt;waypoint&gt;</pre>  
  Gets a waypoint's description  
- <pre class="command-usage-arguments">/waypoints description get-rendered &lt;waypoint&gt;</pre>  
  Gets a waypoint's rendered description  
- <pre class="command-usage-arguments">/waypoints description set &lt;waypoint&gt; &lt;description&gt;</pre>  
  Sets a waypoint's description  
- <pre class="command-usage-arguments">/waypoints creation-date get &lt;waypoint&gt;</pre>  
  Gets a waypoint's creation date  
- <pre class="command-usage-arguments">/waypoints creation-date set &lt;waypoint&gt; &lt;time&gt;</pre>  
  Sets a waypoint's creation date  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:36:30 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 9