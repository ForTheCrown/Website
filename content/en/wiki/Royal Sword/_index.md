---
title: "Royal Sword"
linkTitle: "Royal Sword"
type: docs
weight: 6
description: >
  Information about how Royal Swords work.
---

The Royal Sword is the sword given to all players when 
they first join the server. The sword cannot be dropped, 
but can be levelled up to become more powerful.

# Sword ranks

<table>
  <caption>Sword ranks</caption>

  <thead>
    <tr>
    <td>Ranks</td>
    <td>Goals</td>
    <td>Upgrades/Rewards</td>
    </tr>
  </thead>

  <tbody>
    <!--- 1 -> 2 --->
    <tr>
      <td rowspan=3>1 -> 2</td>
      <td rowspan=3>100 of any entity</td>
      <td>Sword upgraded to stone</td>
    </tr>
    <tr><td>5,000 Rhines</td></tr>
    <tr><td>200 Gems</td></tr>
    <!--- 2 -> 3 --->
    <tr>
     <td rowspan=4> 2 -> 3</td>
     <td>75 Spiders</td>
     <td>Upgrade sword to iron</td>
    </tr>
    <tr>
      <td>150 Skeletons</td>
      <td>800 Rhines</td>
    </tr>
    <tr>
      <td>50 Creepers</td>
      <td rowspan=2>Increased attack damage (+1) and speed (+0.5)</td>
    </tr>
    <tr><td>100 Zombies</td></tr>
    <!--- 3 -> 4 --->
    <tr>
      <td rowspan=4>3 -> 4</td>
      <td>100 Wither Skeletons</td>
      <td>Upgrade sword to diamond</td>
    </tr>
    <tr>
      <td>100 Magma Cubes</td>
      <td>Increased attack damage (+2) and speed (+1)</td>
    </tr>
    <tr>
      <td>100 Blaze</td>
      <td>10,000 Rhines</td>
    </tr>
    <tr>
      <td>100 Piglins</td>
      <td>250 Gems</td>
    </tr>
    <!-- 4 -> 5 --->
    <tr>
      <td rowspan=5>4 -> 5</td>
      <td>Defeat Zhambie (Dungeons Level 1)</td>
      <td>Upgrade sword to gold</td>
    </tr>
    <tr>
      <td>Defeat Skalatan (Dungeons Level 2)</td>
      <td>Looting 4 enchantment</td>
    </tr>
    <tr>
      <td>Defeat Hidey Spidey (Dungeons Level 3)</td>
      <td>Increased attack damage (+5) and speed (+1.5)</td>
    </tr>
    <tr>
      <td rowspan=2>500 of any entity</td>
      <td>10,000 Rhines</td>
    </tr>
    <tr><td>250 Gems</td></tr>
    <!-- 5 -> 6 --->
    <tr>
      <td>5 -> 6</td>
      <td>100 Snow Golems</td>
      <td> -</td>
    </tr>
    <!-- 6 -> 7 --->
    <tr>
      <td rowspan=2>6 -> 7</td>
      <td>120 Ghasts</td>
      <td>12,000 Rhines</td>
    </tr>
    <tr>
      <td>Be a Tier-1 Donator</td>
      <td>250 Gems</td>
    </tr>
    <!-- 7 -> 8 --->
    <tr>
      <td rowspan=2>7 -> 8</td>
      <td rowspan=2>25 Charged Creepers</td>
      <td>15,000 Rhines</td>
    </tr>
    <tr><td>250 Gems</td></tr>
    <!-- 8 -> 9 --->
    <tr>
      <td>8 -> 9</td>
      <td>10 Withers</td>
      <td> -</td>
    </tr>
    <!-- 9 -> 10 --->
    <tr>
      <td rowspan=5>9 -> 10</td>
      <td>300 Endermen</td>
      <td>Sword upgrade to Netherrite</td>
    </tr>
    <tr>
      <td>5 Ender Dragons</td>
      <td>Looting 5 enchantment</td>
    </tr>
    <tr>
      <td rowspan=3>50 Shulkers</td>
      <td>Increased attack damage (+4) and speed (+1.8)</td>
    </tr>
    <tr><td>15,000 Rhines</td></tr>
    <tr><td>250 Gens</td></tr>
    <!--- 10 -> 11 --->
    <tr>
      <td>10 -> 11</td>
      <td>10 Wardens</td>
      <td>-</td>
    </tr>
    <!--- 11 -> 12 --->
    <tr>
      <td rowspan=3>11 -> 12</td>
      <td rowspan=3>25,000 of any entity</td>
      <td>Increased attack damage (+4.4) and speed (+3)</td>
    </tr>
    <tr><td>25,000 Rhines</td></tr>
    <tr><td>450 Gems</td></tr>
    <!--- 12 -> 13 --->
    <tr>
      <td rowspan=3>12 -> 13</td>
      <td rowspan=3>20 Wandering Traders</td>
      <td>Increased attack damage (+4.6) and speed (+3.1)</td>
    </tr>
    <tr><td>25,000 Rhines</td></tr>
    <tr><td>500 Gems</td></tr>
    <!--- 13 -> 14 --->
    <tr>
      <td rowspan=5>13 -> 14</td>
      <td>50 Evokers</td>
      <td>Increased attack damage (4.8) and speed (+3.2)</td>
    </tr>
    <tr>
      <td>250 Pillagers</td>
      <td>35,000 Rhines Gems</td>
    </tr>
    <tr>
      <td>250 Vindicators</td>
      <td rowspan=3>700 Gems</td>
    </tr>
    <tr><td>50 Withers</td></tr>
    <tr><td>50 Ravagers</td></tr>
  </tbody>
</table>

Ranks 14 onwards follow a repeating pattern of rewards and goals.
  
The formula's for those goals are as follows: 
```txt
wither_goal = rank * 1.25
dragon_goal = rank * 1.25
damage_goal = rank * 1000 * 1.25

rhine_reward = rank * 2500
gem_reward = rank * 50
```