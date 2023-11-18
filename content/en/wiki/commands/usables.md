---
title: "usables"
linkTitle: "usables"
type: docs
weight: 1
description: >
  usables commands
---


## /kit
An FTC command (default description)  
  
**Permission**: `ftc.kits`  
**Aliases**: `kits`  
**Uses**:
- <pre class="command-usage-arguments">/kit</pre>  
  Displays a list of Kits  
- <pre class="command-usage-arguments">/kit &lt;kit&gt;</pre>  
  Uses a Kit  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/kit &lt;kit&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  

## /usable
An FTC command (default description)  
  
**Permission**: `ftc.usables`  
**Aliases**: `interactable`, `usables`  
**Uses**:
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; use</pre>  
  Makes you use a block  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; use &lt;players&gt;</pre>  
  Makes a list of players use a block  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usable block &lt;block: x,y,z&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; use</pre>  
  Makes you use a entity  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; use &lt;players&gt;</pre>  
  Makes a list of players use a entity  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usable entity &lt;entity: uuid | @selector&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  
- <pre class="command-usage-arguments">/usable item info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usable item use</pre>  
  Makes you use a item  
- <pre class="command-usage-arguments">/usable item use &lt;players&gt;</pre>  
  Makes a list of players use a item  
- <pre class="command-usage-arguments">/usable item data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usable item data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usable item data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usable item data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usable item data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usable item silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usable item silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usable item actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usable item actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usable item actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable item actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usable item actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usable item actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usable item actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usable item tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usable item tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usable item tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable item tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usable item tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usable item tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usable item tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  
- <pre class="command-usage-arguments">/usable triggers create &lt;name&gt;</pre>  
  Defines a new trigger, using your world edit  
  selection as the trigger's area  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; rename &lt;trigger name&gt; &lt;new name&gt;</pre>  
  Renames a trigger to name  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; redefine &lt;trigger name&gt;</pre>  
  Redefines a trigger to your current world edit selection  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; remove</pre>  
  Removes a trigger  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; use</pre>  
  Makes you use a triggers  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; use &lt;players&gt;</pre>  
  Makes a list of players use a triggers  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usable triggers &lt;trigger&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  
- <pre class="command-usage-arguments">/usable kit</pre>  
  Displays a list of Kits  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt;</pre>  
  Uses a Kit  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usable kit &lt;kit&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  
- <pre class="command-usage-arguments">/usable warp</pre>  
  Displays a list of Warps  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; destination</pre>  
  Displays a warp's current destination location  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; destination set</pre>  
  Sets a warp's destination to where you're standing  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; destination set &lt;pos: x,y,z&gt;</pre>  
  Sets a warp's position to the given xyz coordinates  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; instant</pre>  
  Shows if a warp will always instantly teleport players or not  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; instant &lt;true | false&gt;</pre>  
  Sets if a warp will always instantly teleport players or not  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt;</pre>  
  Uses a Warp  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usable warp &lt;warp&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  

## /usableblock
An FTC command (default description)  
  
**Permission**: `ftc.usables.block`  
**Aliases**: `usable_block`  
**Uses**:
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; use</pre>  
  Makes you use a block  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; use &lt;players&gt;</pre>  
  Makes a list of players use a block  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usableblock &lt;block: x,y,z&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  

## /usableentity
An FTC command (default description)  
  
**Permission**: `ftc.usables.entity`  
**Aliases**: `usable_entity`  
**Uses**:
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; use</pre>  
  Makes you use a entity  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; use &lt;players&gt;</pre>  
  Makes a list of players use a entity  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usableentity &lt;entity: uuid | @selector&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  

## /usableitem
An FTC command (default description)  
  
**Permission**: `ftc.usables.item`  
**Aliases**: `usable_item`  
**Uses**:
- <pre class="command-usage-arguments">/usableitem info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usableitem use</pre>  
  Makes you use a item  
- <pre class="command-usage-arguments">/usableitem use &lt;players&gt;</pre>  
  Makes a list of players use a item  
- <pre class="command-usage-arguments">/usableitem data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usableitem data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usableitem data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usableitem data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usableitem data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usableitem silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usableitem silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usableitem actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usableitem actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usableitem actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usableitem actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usableitem actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usableitem actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usableitem actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usableitem tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usableitem tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usableitem tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usableitem tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usableitem tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usableitem tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usableitem tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  

## /usabletriggers
An FTC command (default description)  
  
**Permission**: `ftc.usables.trigger`  
**Aliases**: `usable_triggers`, `triggers`  
**Uses**:
- <pre class="command-usage-arguments">/usabletriggers create &lt;name&gt;</pre>  
  Defines a new trigger, using your world edit  
  selection as the trigger's area  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; rename &lt;trigger name&gt; &lt;new name&gt;</pre>  
  Renames a trigger to name  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; redefine &lt;trigger name&gt;</pre>  
  Redefines a trigger to your current world edit selection  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; remove</pre>  
  Removes a trigger  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; use</pre>  
  Makes you use a triggers  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; use &lt;players&gt;</pre>  
  Makes a list of players use a triggers  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/usabletriggers &lt;trigger&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  

## /warp
An FTC command (default description)  
  
**Permission**: `ftc.warps`  
**Aliases**: `warps`  
**Uses**:
- <pre class="command-usage-arguments">/warp</pre>  
  Displays a list of Warps  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; destination</pre>  
  Displays a warp's current destination location  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; destination set</pre>  
  Sets a warp's destination to where you're standing  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; destination set &lt;pos: x,y,z&gt;</pre>  
  Sets a warp's position to the given xyz coordinates  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; instant</pre>  
  Shows if a warp will always instantly teleport players or not  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; instant &lt;true | false&gt;</pre>  
  Sets if a warp will always instantly teleport players or not  
- <pre class="command-usage-arguments">/warp &lt;warp&gt;</pre>  
  Uses a Warp  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; info</pre>  
  Shows general info  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; data</pre>  
  Displays the Usable data  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; data view [&lt;path: nbt path&gt;]</pre>  
  Displays Usable data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Usable data at a path  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; data merge &lt;tag&gt;</pre>  
  Merges a tag into Usable data  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Usable data  
  and sets it to tag  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; silent</pre>  
  Checks if a usable is silent  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; silent &lt;true | false&gt;</pre>  
  Sets a usable to be silent or not  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; actions</pre>  
  Shows all the existing Actions  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; actions clear</pre>  
  Clears the Action list  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; actions remove &lt;indices&gt;</pre>  
  Removes a Action  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; actions add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; actions add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Action before the element at index  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; actions add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Action to the front of the Actions list  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; actions set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Action at index to type  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; tests</pre>  
  Shows all the existing Conditions  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; tests clear</pre>  
  Clears the Condition list  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; tests remove &lt;indices&gt;</pre>  
  Removes a Condition  
  Examples:  
  - remove 1: Removes an element at index 1  
  - remove 1..3: Removes all elements between indices 1 through 3  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; tests add &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; tests add -at &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds an Condition before the element at index  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; tests add -first &lt;type&gt; [&lt;input&gt;]</pre>  
  Adds a Condition to the front of the Conditions list  
- <pre class="command-usage-arguments">/warp &lt;warp&gt; tests set &lt;index&gt; &lt;type&gt; [&lt;input&gt;]</pre>  
  Sets the Condition at index to type  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 7