---
title: "Sell Shop"
linkTitle: "Sell Shop"
type: docs
math: true
weight: 5
description: >
  SellShop wiki
---
## What is the sell shop
The sell shop is a shop where players can sell items for rhines. It can be opened with
 `/shop`  
  
The sell shop is made of 4 parts: Mob Drops, Minerals, Mining, Crops. You can 
quickly access these parts by using `/shop drops`, `/shop minerals`, 
`/shop mining` or `/shop crops`.

## Menus
<img src="/images/sell_shop/main.png" alt="Sellshop main menu">  

### Buttons
<img src="/images/sell_shop/buttons.png" alt="Sellshop Buttons guide">  

<img src="/images/sell_shop/compact.png" alt="Sellshop Compact guide">  

<img src="/images/sell_shop/amounts.png" alt="Sellshop Sell amounts guide">  
  
### Mob drops menu
<img src="/images/sell_shop/drops.png" alt="Sellshop Drops menu">  

### Regular items
Material | Base price | Max earnings
|--|--|--|
String | 2 | 500,000
Magma Cream | 5 | 500,000
Slimeball | 4 | 500,000
Arrow | 5 | 500,000
Gunpowder | 5 | 500,000
Leather | 10 | 500,000
Raw Cod | 3 | 500,000
Ink Sac | 5 | 500,000
Bone | 2 | 500,000
Rotten Flesh | 2 | 500,000
Blaze Rod | 5 | 500,000
Spider Eye | 5 | 500,000

### Compact items
Material | Base price | Max earnings
|--|--|--|
White Wool | 8 | 500,000
Magma Block | 20 | 500,000
Slime Block | 36 | 500,000

### Minerals menu  
<img src="/images/sell_shop/minerals.png" alt="Sellshop Minerals menu">  

### Regular items
Material | Base price | Max earnings
|--|--|--|
Coal | 10 | 500,000
Amethyst Shard | 8 | 500,000
Iron Ingot | 5 | 500,000
Copper Ingot | 8 | 500,000
Gold Ingot | 7 | 500,000
Diamond | 400 | 500,000
Netherite Ingot | 8,000 | 500,000
Lapis Lazuli | 10 | 500,000
Emerald | 7 | 500,000
Nether Quartz | 3 | 500,000
Redstone Dust | 10 | 500,000


### Compact items
Material | Base price | Max earnings
|--|--|--|
Block of Coal | 90 | 500,000
Block of Amethyst | 32 | 500,000
Block of Iron | 45 | 500,000
Block of Copper | 72 | 500,000
Block of Gold | 63 | 500,000
Block of Diamond | 3,600 | 500,000
Block of Netherite | 72,000 | 500,000
Block of Lapis Lazuli | 90 | 500,000
Block of Emerald | 63 | 500,000
Block of Quartz | 12 | 500,000
Block of Redstone | 90 | 500,000

### Mining menu
<img src="/images/sell_shop/mining.png" alt="Sellshop Mining menu">  

### Regular items
Material | Base price | Max earnings
|--|--|--|
Stone | 2 | 500,000
Granite | 3 | 500,000
Diorite | 3 | 500,000
Andesite | 3 | 500,000
Deepslate | 2 | 500,000
Cobbled Deepslate | 2 | 500,000
Tuff | 5 | 500,000
Dirt | 2 | 500,000
Cobblestone | 2 | 500,000
Sand | 2 | 500,000
Gravel | 2 | 500,000
Netherrack | 2 | 500,000
Basalt | 3 | 500,000
Smooth Basalt | 3 | 500,000
End Stone | 3 | 500,000
Blackstone | 3 | 500,000

### Compact items
Material | Base price | Max earnings
|--|--|--|
Sandstone | 8 | 500,000

### Farming menu
<img src="/images/sell_shop/farming.png" alt="Sellshop Farming menu">  
  
### Regular items
Material | Base price | Max earnings
|--|--|--|
Sugar Cane | 3 | 500,000
Kelp | 2 | 500,000
Cactus | 2 | 500,000
Pumpkin | 3 | 500,000
Melon | 8 | 500,000
Wheat | 7 | 500,000
Stick | 4 | 500,000
Wheat Seeds | 3 | 500,000
Carrot | 4 | 500,000
Potato | 4 | 500,000
Chorus Fruit | 10 | 500,000
Torchflower Seeds | 10 | 500,000
Pitcher Pod | 10 | 500,000
Sweet Berries | 5 | 500,000
Honeycomb | 6 | 500,000

### Compact items
Material | Base price | Max earnings
|--|--|--|
Paper | 3 | 500,000
Hay Bale | 63 | 500,000
Honeycomb Block | 24 | 500,000


## Price Decrease (Info for nerds)
Prices in the sell shop will decrease when you sell items. The price will 
recover over time.
  
The price decrease is based off how much you've earned from a single item.
An item's price is calculated using a function which is defined as follows:
  
$$f(x) =\text{ceil}\left(A\cdot\arctan\left(Bx-C\right)+D\right)$$
  
\\(m = 250000\\) (Max you can earn from an item, may vary based on item)  
\\(s = initalPrice\\)  
\\(B = 0.00015\\)  
\\(C = \frac{Bm}{2}\\)  
\\(D = \frac{s}{2}\\)  
\\(A = \frac{-s}{2\arctan\left(C\right)}\\)  
  
The input, \\(x\\), is the current amount of rhines already earned from the 
item.
  
To see this function visualized, Checkout [The Desmos Graph](https://www.desmos.com/calculator/77bahmzgew)
  
Each item's earnings will be decreased by 5000 (Correct as of 09-09-2023) each 
day, allowing your price to slowly recover over time. This recalculation is triggered each time you join the server.
