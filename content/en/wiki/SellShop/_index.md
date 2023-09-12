---
title: "Sell Shop"
linkTitle: "Sell Shop"
type: docs
weight: 5
description: >
  SellShop wiki
---
# What is the sell shop
The sell shop is a shop where players can sell items for rhines. It can be opened with
 `/shop`  
  
The sell shop is made of 4 parts: Mob Drops, Minerals, Mining, Crops. You can 
quickly access these parts by using `/shop drops`, `/shop minerals`, 
`/shop mining` or `/shop crops`.

# Menus
<img src="/images/sell_shop/main.png" alt="Sellshop main menu">  

## Buttons
<img src="/images/sell_shop/buttons.png" alt="Sellshop Buttons guide">  

<img src="/images/sell_shop/compact.png" alt="Sellshop Compact guide">  

<img src="/images/sell_shop/amounts.png" alt="Sellshop Sell amounts guide">  
  
## Mob drops menu
<img src="/images/sell_shop/drops.png" alt="Sellshop Drops menu">  

## Minerals menu  
<img src="/images/sell_shop/minerals.png" alt="Sellshop Minerals menu">  

## Mining menu
<img src="/images/sell_shop/mining.png" alt="Sellshop Mining menu">  

## Farming menu
<img src="/images/sell_shop/farming.png" alt="Sellshop Farming menu">  
  
# Price Decrease (Info for nerds)
Prices in the sell shop will decrease when you sell items. The price will 
recover over time.
  
The price decrease is based off how much you've earned from a single item.
An item's price is calculated using a function which is defined as follows:
  
$f\left(x\right)\ =\operatorname{ceil}\left(A\cdot\arctan\left(Bx-C\right)+D\right)$

$m = 250000$ (Max you can earn from an item, may vary based on item)  
$s = initalPrice$  
$B = 0.00015$  
$C = \frac{Bm}{2}$  
$D = \frac{s}{2}$  
$A = \frac{-s}{2\arctan\left(C\right)}$  
  
The input, $x$, is the current amount of rhines already earned from the 
item.
  
To see this function visualized, Checkout [The Desmos Graph](https://www.desmos.com/calculator/77bahmzgew)
  
Each item's earnings will be decreased by 5000 (Correct as of 09-09-2023) each 
day, allowing your price to slowly recover over time. This recalculation is triggered each time you join the server.