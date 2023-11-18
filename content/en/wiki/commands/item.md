---
title: "item"
linkTitle: "item"
type: docs
weight: 1
description: >
  item commands
---


## /enchant
An FTC command (default description)  
  
**Permission**: `ftc.commands.items`  
**Uses**:
- <pre class="command-usage-arguments">/enchant &lt;enchantment&gt; [&lt;level: number(1..)&gt;]</pre>  
  Applies the enchantment to your held item  
  with [level]. If [level] is not given, then  
  a level of 1 is used.  
  If the item is a book, enchanting it turns it  
  into an enchanted book  
- <pre class="command-usage-arguments">/enchant clear</pre>  
  Clears all your held item's enchantments  

## /item_attribute_modifiers
An FTC command (default description)  
  
**Permission**: `ftc.commands.items`  
**Uses**:
- <pre class="command-usage-arguments">/item_attribute_modifiers clear</pre>  
  Clears the item's Attribute Modifiers  
- <pre class="command-usage-arguments">/item_attribute_modifiers remove &lt;attribute&gt;</pre>  
  Removes all modifiers which modify the  
  attribute value  
- <pre class="command-usage-arguments">/item_attribute_modifiers remove attr &lt;attribute&gt;</pre>  
  Same as above  
- <pre class="command-usage-arguments">/item_attribute_modifiers remove slot &lt;equipment slot&gt;</pre>  
  Removes all modifiers which apply to the  
  equipment slot  

## /item_cooldown
An FTC command (default description)  
  
**Permission**: `ftc.commands.items`  
**Aliases**: `itemcooldown`  
**Uses**:
- <pre class="command-usage-arguments">/item_cooldown &lt;material&gt;</pre>  
  Shows how long a material is on cooldown for you  
- <pre class="command-usage-arguments">/item_cooldown &lt;material&gt; &lt;time&gt;</pre>  
  Sets your material's cooldown to time  

## /item_data
An FTC command (default description)  
  
**Permission**: `ftc.commands.items`  
**Aliases**: `item_tags`, `itemnbt`, `itemdata`, `itemtags`  
**Uses**:
- <pre class="command-usage-arguments">/item_data give_command</pre>  
  Creates a `/give` command for the item you're holding  
- <pre class="command-usage-arguments">/item_data</pre>  
  Displays the Item data  
- <pre class="command-usage-arguments">/item_data view [&lt;path: nbt path&gt;]</pre>  
  Displays Item data, if [path] is set, shows only  
  data at that path  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  
- <pre class="command-usage-arguments">/item_data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Item data at a path  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  
- <pre class="command-usage-arguments">/item_data merge &lt;tag&gt;</pre>  
  Merges a tag into Item data  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  
- <pre class="command-usage-arguments">/item_data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Item data  
  and sets it to tag  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  

## /itemname
An FTC command (default description)  
  
**Permission**: `ftc.commands.items`  
**Aliases**: `nameitem`, `renameitem`, `itemrename`  
**Uses**:
- <pre class="command-usage-arguments">/itemname &lt;text&gt;</pre>  
  Sets the name of the item you're holding  
  Note:  
  If the text is a JSON component (eg: {"text":"Item Name"})  
  The name won't automatically become non-italic  
  and white, you'll be required to manually set them to  
  that configuration  
- <pre class="command-usage-arguments">/itemname -clear</pre>  
  Clears the name of the item you're holding  

## /items
An FTC command (default description)  
  
**Permission**: `ftc.commands.items`  
**Aliases**: `itemstacks`, `itemstack`, `item`  
**Uses**:
- <pre class="command-usage-arguments">/items enchant &lt;enchantment&gt; [&lt;level: number(1..)&gt;]</pre>  
  Applies the enchantment to your held item  
  with [level]. If [level] is not given, then  
  a level of 1 is used.  
  If the item is a book, enchanting it turns it  
  into an enchanted book  
- <pre class="command-usage-arguments">/items enchant clear</pre>  
  Clears all your held item's enchantments  
- <pre class="command-usage-arguments">/items lore clear</pre>  
  Clears your held item's lore  
- <pre class="command-usage-arguments">/items lore add &lt;text&gt;</pre>  
  Adds text to your held item's lore  
  Note:  
  If the text is a JSON component (eg: {"text":"Item Name"})  
  The name won't automatically become non-italic  
  and white, you'll be required to manually set them to  
  that configuration  
- <pre class="command-usage-arguments">/items lore display</pre>  
  Displays the lore of the item you're holding with index numbers  
- <pre class="command-usage-arguments">/items lore set &lt;index&gt; &lt;text&gt;</pre>  
  Sets the lore on the specified line of the item you're holding  
- <pre class="command-usage-arguments">/items lore remove &lt;index&gt;</pre>  
  Removes the lore on the given line  
- <pre class="command-usage-arguments">/items lore remove at &lt;index&gt;</pre>  
  Removes the lore on the given line  
- <pre class="command-usage-arguments">/items lore remove between &lt;start index&gt; &lt;end index&gt;</pre>  
  Removes all lore between the 2 lines  
- <pre class="command-usage-arguments">/items name &lt;text&gt;</pre>  
  Sets the name of the item you're holding  
  Note:  
  If the text is a JSON component (eg: {"text":"Item Name"})  
  The name won't automatically become non-italic  
  and white, you'll be required to manually set them to  
  that configuration  
- <pre class="command-usage-arguments">/items name -clear</pre>  
  Clears the name of the item you're holding  
- <pre class="command-usage-arguments">/items data give_command</pre>  
  Creates a `/give` command for the item you're holding  
- <pre class="command-usage-arguments">/items data</pre>  
  Displays the Item data  
- <pre class="command-usage-arguments">/items data view [&lt;path: nbt path&gt;]</pre>  
  Displays Item data, if [path] is set, shows only  
  data at that path  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  
- <pre class="command-usage-arguments">/items data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Item data at a path  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  
- <pre class="command-usage-arguments">/items data merge &lt;tag&gt;</pre>  
  Merges a tag into Item data  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  
- <pre class="command-usage-arguments">/items data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Item data  
  and sets it to tag  
  Note: the tag and path roots are the item's raw NBT  
  Not the 'tag' element.  
- <pre class="command-usage-arguments">/items attributes clear</pre>  
  Clears the item's Attribute Modifiers  
- <pre class="command-usage-arguments">/items attributes remove &lt;attribute&gt;</pre>  
  Removes all modifiers which modify the  
  attribute value  
- <pre class="command-usage-arguments">/items attributes remove attr &lt;attribute&gt;</pre>  
  Same as above  
- <pre class="command-usage-arguments">/items attributes remove slot &lt;equipment slot&gt;</pre>  
  Removes all modifiers which apply to the  
  equipment slot  
- <pre class="command-usage-arguments">/items cooldown &lt;material&gt;</pre>  
  Shows how long a material is on cooldown for you  
- <pre class="command-usage-arguments">/items cooldown &lt;material&gt; &lt;time&gt;</pre>  
  Sets your material's cooldown to time  

## /lore
An FTC command (default description)  
  
**Permission**: `ftc.commands.items`  
**Aliases**: `itemlore`, `lores`, `itemlores`  
**Uses**:
- <pre class="command-usage-arguments">/lore clear</pre>  
  Clears your held item's lore  
- <pre class="command-usage-arguments">/lore add &lt;text&gt;</pre>  
  Adds text to your held item's lore  
  Note:  
  If the text is a JSON component (eg: {"text":"Item Name"})  
  The name won't automatically become non-italic  
  and white, you'll be required to manually set them to  
  that configuration  
- <pre class="command-usage-arguments">/lore display</pre>  
  Displays the lore of the item you're holding with index numbers  
- <pre class="command-usage-arguments">/lore set &lt;index&gt; &lt;text&gt;</pre>  
  Sets the lore on the specified line of the item you're holding  
- <pre class="command-usage-arguments">/lore remove &lt;index&gt;</pre>  
  Removes the lore on the given line  
- <pre class="command-usage-arguments">/lore remove at &lt;index&gt;</pre>  
  Removes the lore on the given line  
- <pre class="command-usage-arguments">/lore remove between &lt;start index&gt; &lt;end index&gt;</pre>  
  Removes all lore between the 2 lines  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 7