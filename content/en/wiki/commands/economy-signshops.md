---
title: "economy/signshops"
linkTitle: "economy/signshops"
type: docs
weight: 1
description: >
  economy/signshops commands
---


## /editshop
Allows you to edit a shop  
  
**Permission**: `ftc.commands.shopedit`  
**Aliases**: `shopedit`, `signshop`  
**Uses**:
- <pre class="command-usage-arguments">/editshop</pre>  
  Displays help information  
- <pre class="command-usage-arguments">/editshop buy</pre>  
  Makes the shop you're looking at a buy shop  
- <pre class="command-usage-arguments">/editshop sell</pre>  
  Makes the shop you're looking at a sell shop  
- <pre class="command-usage-arguments">/editshop line &lt;2 | 3&gt; &lt;text&gt;</pre>  
  Changes either the 2nd or 3rd line of the  
  sign shop you're looking at  
- <pre class="command-usage-arguments">/editshop amount &lt;amount: number(1..64)&gt;</pre>  
  Changes the amount of items the shop sells/buys  
- <pre class="command-usage-arguments">/editshop price &lt;value: number(1..)&gt;</pre>  
  Changes the price of the shop you're looking at  
- <pre class="command-usage-arguments">/editshop info</pre>  
  Displays info about the shop you're looking at  
- <pre class="command-usage-arguments">/editshop data</pre>  
  Displays the Shop data  
- <pre class="command-usage-arguments">/editshop data view [&lt;path: nbt path&gt;]</pre>  
  Displays Shop data, if [path] is set, shows only  
  data at that path  
- <pre class="command-usage-arguments">/editshop data insert &lt;path: nbt path&gt; &lt;tag&gt;</pre>  
  Inserts a tag into Shop data at a path  
- <pre class="command-usage-arguments">/editshop data merge &lt;tag&gt;</pre>  
  Merges a tag into Shop data  
- <pre class="command-usage-arguments">/editshop data set &lt;tag&gt;</pre>  
  Completely overwrites the existing Shop data  
  and sets it to tag  

## /shophistory
Shows the history of the shop you're looking at  
  
**Permission**: `ftc.commands.shophistory`  
**Uses**:
- <pre class="command-usage-arguments">/shophistory</pre>  
  Shows the history of the shop you're looking at  

## /shopreselling
Shop reselling  
  
**Permission**: `ftc.default`  
**Aliases**: `shopresell`  
**Uses**:
- <pre class="command-usage-arguments">/shopreselling</pre>  
  Shop reselling  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 3