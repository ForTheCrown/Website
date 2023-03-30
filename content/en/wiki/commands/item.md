---
title: "Item"
linkTitle: "Item"
type: docs
weight: 1
description: >
  Item Commands
---

# Table of Contents
- [/enchant](#commands_item_EnchantmentNode)
- [/item_attribute_modifiers](#commands_item_ItemAttributeNode)
- [/item_cooldown](#commands_item_ItemCooldownNode)
- [/item_data](#commands_item_ItemDataNode)
- [/itemname](#commands_item_ItemNameNode)
- [/items](#commands_item_ItemModCommands$ItemStacksCommand)
- [/lore](#commands_item_ItemLoreNode)

# Commands
## /enchant <a name="commands_item_EnchantmentNode"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/enchant <enchantment> [<level: number(1..)>]
# Applies the <enchantment> to your held item
# with [level]. If [level] is not given, then
# a level of 1 is used.
# If the item is a book, enchanting it turns it
# into an enchanted book

/enchant clear
# Clears all your held item's enchantments
```

## /item_attribute_modifiers <a name="commands_item_ItemAttributeNode"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
### Usages
```yaml
/item_attribute_modifiers clear
# Clears the item's Attribute Modifiers

/item_attribute_modifiers remove <attribute>
# Removes all modifiers which modify the
# <attribute> value

/item_attribute_modifiers remove attr <attribute>
# Same as above

/item_attribute_modifiers remove slot <equipment slot>
# Removes all modifiers which apply to the
# <equipment slot>
```

## /item_cooldown <a name="commands_item_ItemCooldownNode"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `itemcooldown`  
### Usages
```yaml
/item_cooldown <material>
# Shows how long a <material> is on cooldown for you

/item_cooldown <material> <time>
# Sets your <material>'s cooldown to <time>
```

## /item_data <a name="commands_item_ItemDataNode"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `item_tags`, `itemnbt`, `itemdata`, `itemtags`  
### Usages
```yaml
/item_data
# Displays the Item data

/item_data view [<path: nbt path>]
# Displays Item data, if [path] is set, shows only
# data at that path
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.

/item_data insert <path: nbt path> <tag>
# Inserts a <tag> into Item data at a <path>
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.

/item_data merge <tag>
# Merges a <tag> into Item data
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.

/item_data set <tag>
# Completely overwrites the existing Item data
# and sets it to <tag>
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.
```

## /itemname <a name="commands_item_ItemNameNode"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `nameitem`, `renameitem`, `itemrename`  
### Usages
```yaml
/itemname <text>
# Sets the name of the item you're holding
# Note:
# If the <text> is a JSON component (eg: {"text":"Item Name"})
# The name won't automatically become non-italic
# and white, you'll be required to manually set them to
# that configuration

/itemname -clear
# Clears the name of the item you're holding
```

## /items <a name="commands_item_ItemModCommands$ItemStacksCommand"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `itemstacks`, `itemstack`, `item`  
### Usages
```yaml
/items enchant <enchantment> [<level: number(1..)>]
# Applies the <enchantment> to your held item
# with [level]. If [level] is not given, then
# a level of 1 is used.
# If the item is a book, enchanting it turns it
# into an enchanted book

/items enchant clear
# Clears all your held item's enchantments

/items lore clear
# Clears your held item's lore

/items lore add <text>
# Adds <text> to your held item's lore
# Note:
# If the <text> is a JSON component (eg: {"text":"Item Name"})
# The name won't automatically become non-italic
# and white, you'll be required to manually set them to
# that configuration

/items lore remove <index>
# Removes the lore on the given line

/items lore remove at <index>
# Removes the lore on the given line

/items lore remove between <start index> <end index>
# Removes all lore between the 2 lines

/items name <text>
# Sets the name of the item you're holding
# Note:
# If the <text> is a JSON component (eg: {"text":"Item Name"})
# The name won't automatically become non-italic
# and white, you'll be required to manually set them to
# that configuration

/items name -clear
# Clears the name of the item you're holding

/items data
# Displays the Item data

/items data view [<path: nbt path>]
# Displays Item data, if [path] is set, shows only
# data at that path
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.

/items data insert <path: nbt path> <tag>
# Inserts a <tag> into Item data at a <path>
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.

/items data merge <tag>
# Merges a <tag> into Item data
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.

/items data set <tag>
# Completely overwrites the existing Item data
# and sets it to <tag>
# Note: the <tag> and <path> roots are the item's raw NBT
# Not the 'tag' element.

/items attributes clear
# Clears the item's Attribute Modifiers

/items attributes remove <attribute>
# Removes all modifiers which modify the
# <attribute> value

/items attributes remove attr <attribute>
# Same as above

/items attributes remove slot <equipment slot>
# Removes all modifiers which apply to the
# <equipment slot>

/items cooldown <material>
# Shows how long a <material> is on cooldown for you

/items cooldown <material> <time>
# Sets your <material>'s cooldown to <time>
```

## /lore <a name="commands_item_ItemLoreNode"></a>
An FTC command (default description)  
  
**Command metadata**:  
Permission: `ftc.admin`  
Aliases: `itemlore`, `lores`, `itemlores`  
### Usages
```yaml
/lore clear
# Clears your held item's lore

/lore add <text>
# Adds <text> to your held item's lore
# Note:
# If the <text> is a JSON component (eg: {"text":"Item Name"})
# The name won't automatically become non-italic
# and white, you'll be required to manually set them to
# that configuration

/lore remove <index>
# Removes the lore on the given line

/lore remove at <index>
# Removes the lore on the given line

/lore remove between <start index> <end index>
# Removes all lore between the 2 lines
```

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Thu Mar 30 22:08:46 CEST 2023`  
Plugin version: `1.19.4-1733-RELEASE`  
Total commands: 7