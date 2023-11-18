---
title: "leaderboards"
linkTitle: "leaderboards"
type: docs
weight: 1
description: >
  leaderboards commands
---


## /leaderboards
Leaderboards admin command  
  
**Permission**: `ftc.commands.leaderboards`  
**Aliases**: `lb`  
**Uses**:
- <pre class="command-usage-arguments">/leaderboards reload-config</pre>  
  Reloads the Leaderboards Config  
- <pre class="command-usage-arguments">/leaderboards reload-boards</pre>  
  Reloads all leaderboards from disc  
- <pre class="command-usage-arguments">/leaderboards save</pre>  
  Saves all leaderboards to disk  
- <pre class="command-usage-arguments">/leaderboards list</pre>  
  Lists all leaderboards  
- <pre class="command-usage-arguments">/leaderboards list [&lt;page size&gt;] [&lt;page size&gt;]</pre>  
  Lists all leaderboards on a specific page  
- <pre class="command-usage-arguments">/leaderboards create &lt;name&gt;</pre>  
  Creates a new leaderboard with 'dummy' source  
- <pre class="command-usage-arguments">/leaderboards info &lt;board&gt;</pre>  
  Shows info about a leaderboard  
- <pre class="command-usage-arguments">/leaderboards update &lt;board&gt;</pre>  
  Updates a leaderboard  
- <pre class="command-usage-arguments">/leaderboards update-all</pre>  
  Updates all leaderboards  
- <pre class="command-usage-arguments">/leaderboards kill &lt;board&gt;</pre>  
  Kills a leaderboard  
- <pre class="command-usage-arguments">/leaderboards remove &lt;board&gt;</pre>  
  Kills and deletes a leaderboard  
- <pre class="command-usage-arguments">/leaderboards spawn &lt;board&gt;</pre>  
  Spawns a leaderboard  
- <pre class="command-usage-arguments">/leaderboards location &lt;board&gt;</pre>  
  Moves a leaderboard to where you're standing  
- <pre class="command-usage-arguments">/leaderboards location &lt;board&gt; &lt;pos: x y z&gt;</pre>  
  Moves a leaderboard to the specified xyz coordinates  
- <pre class="command-usage-arguments">/leaderboards footer &lt;board&gt; &lt;text&gt;</pre>  
  Sets the footer used by a leaderboard  
- <pre class="command-usage-arguments">/leaderboards header &lt;board&gt; &lt;text&gt;</pre>  
  Sets the header (title) used by a leaderboard  
- <pre class="command-usage-arguments">/leaderboards format &lt;board&gt; &lt;text&gt;</pre>  
  Sets the format used by a leaderboard  
- <pre class="command-usage-arguments">/leaderboards you-format set &lt;board&gt; &lt;text&gt;</pre>  
  Sets the format used when displaying the 'You' entry  
- <pre class="command-usage-arguments">/leaderboards you-format unset &lt;board&gt;</pre>  
  Reverts the format used for displaying the 'You' entry  
  back to the regular format  
- <pre class="command-usage-arguments">/leaderboards include-you &lt;board&gt; &lt;value&gt;</pre>  
  Enables/Disables the 'You' entry being displayed  
    
  The 'You' entry will not be shown if a non-player leaderboard  
  is being rendered, or if the player has no score in the leaderboard  
- <pre class="command-usage-arguments">/leaderboards order &lt;board&gt; &lt;order&gt;</pre>  
  Sets the order in which elements are listed  
- <pre class="command-usage-arguments">/leaderboards source &lt;board&gt; &lt;source&gt;</pre>  
  Sets the data source used by a leaderboard  
- <pre class="command-usage-arguments">/leaderboards max-size &lt;board&gt; &lt;size&gt;</pre>  
  Sets the maximum amount of entries a leaderboard will show  
- <pre class="command-usage-arguments">/leaderboards fill-empty &lt;board&gt; &lt;value&gt;</pre>  
  Sets whether the leaderboard size is changed or if empty  
  slots are filled with '-' values  
- <pre class="command-usage-arguments">/leaderboards filter set &lt;board&gt; &lt;filter&gt;</pre>  
  Sets a leaderboard's score filter  
- <pre class="command-usage-arguments">/leaderboards filter unset &lt;board&gt;</pre>  
  Removes a leaderboard's filter  
- <pre class="command-usage-arguments">/leaderboards entity yaw &lt;board&gt; &lt;value&gt;</pre>  
  Sets the yaw (x rotation) of a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity pitch &lt;board&gt; &lt;value&gt;</pre>  
  Sets the pitch (y rotation) of a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity scale set &lt;board&gt; &lt;value&gt;</pre>  
  Sets a leaderboard's scale  
- <pre class="command-usage-arguments">/leaderboards entity scale unset &lt;board&gt;</pre>  
  Removes a set scale value from a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity translation set &lt;board&gt; &lt;value&gt;</pre>  
  Sets the transformation offset of a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity translation unset &lt;board&gt;</pre>  
  Removes a set offset value from a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity billboard &lt;board&gt; &lt;value&gt;</pre>  
  Sets the 'billboard' value of a leaderboard  
  A 'billboard' decides if a leaderboard is always rotated to face you  
  or is at a fixed angle  
- <pre class="command-usage-arguments">/leaderboards entity text-align &lt;board&gt; &lt;value&gt;</pre>  
  Sets the text alignment of a leaderboard (left, right, or center)  
- <pre class="command-usage-arguments">/leaderboards entity background-color set &lt;board&gt; &lt;value&gt;</pre>  
  Sets the background color of a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity background-color unset &lt;board&gt;</pre>  
  Removes a set background color value from a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity brightness set &lt;board&gt; &lt;skylight&gt; &lt;blocklight&gt;</pre>  
  Sets the 'brightness' of a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity brightness unset &lt;board&gt;</pre>  
  Removes a set 'brightness' value from a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity shadowed &lt;board&gt; &lt;true|false&gt;</pre>  
  Sets the background color of a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity see-through &lt;board&gt; &lt;value&gt;</pre>  
  Sets if a leaderboard can be seen through  
- <pre class="command-usage-arguments">/leaderboards entity line-width set &lt;board&gt; &lt;value&gt;</pre>  
  Sets a leaderboard's line width  
- <pre class="command-usage-arguments">/leaderboards entity line-width unset &lt;board&gt;</pre>  
  Removes a leaderboard's set line-width value  
- <pre class="command-usage-arguments">/leaderboards entity text-opacity set &lt;board&gt; &lt;value&gt;</pre>  
  Sets the text opacity of a leaderboard  
- <pre class="command-usage-arguments">/leaderboards entity text-opacity unset &lt;board&gt;</pre>  
  Removes the set text opacity value of leaderboard  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 1