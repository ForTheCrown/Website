---
title: "Scripting"
linkTitle: "Scripting"
description: >
  This section explains how scripts can be used to handle logic of challenges.
---

{{% pageinfo %}}
Script files are stored in `plugins/ForTheCrown/scripts` as `.js` files.  
{{% /pageinfo %}}

Note: Be aware that script files are reloaded when they are deactivated/activated, so any data stored in the scripts themselves will be lost.


## ChallengeHandle
Before talking about any implementation details, You should know about the `ChallengeHandle` class. This class allows for giving rewards.

Class methods:

---
```java
void givePoint(Object player);
```
**Description**:  
Gives a single point to the player.
  
**Params**:
- `player`: The player object, can be a player, UUID, User, or the player's name.
---
```java
void givePoints(Object player, float points);
```
**Description**:  
Gives the player the given amount of points.  
  
**Params**:
- `player`: The player object, can be a player, UUID, User, or the player's name.
- `points`: The number of points to give the player.
---
```java
boolean hasCompleted(Object player);
```
**Description**:  
Tests if the given player has completed this handle's challenge.  
  
**Params**:
- `player`: The player object, can be a player, UUID, User, or the player's name.
## Implementation methods
This section specifies methods that can be implemented by challenge scripts
```js
// Called to handle the event logic for this challenge,
// If this method is not specified then the player in the
// event is simply given 1 point.
// If the challenge has a 'custom' event class, the first
// parameter will be an arbitrary object that's given as
// input by the discretion of whoever is writing this lol.
// 
// Params:
// event - The event this challenge is listening to
// handle - The challenge's ChallengeHandle
function onEvent(event, handle);

// This will only be called if onEvent() has not been specified,
// This gets the player in the given event, if this method is not
// specified then the system will attempt to get the player automatically,
// by casting it to a PlayerEvent, if that doesn't work, it fails.
// Params:
// event - The event to get the player of.
// 
// Return: The player event's player
function getPlayer(event);

// Tests if the given User object can complete the challenge
// Params:
// user - The user to test
//
// Return: True, if the user is allowed to complete the 
// 		   challenge, false otherwise
function canComplete(user);

// Called when the player completes this challenge
// Params:
// user - The User that completed this challenge
function onComplete(user);

// Called when the challenge's listeners are registered
// and it becomes 'active' 
// Included for the reason that during the daily reset,
// challenges may be changed, reset, new ones added, and
// this acts as a callback during that time.
// As an example, this is used in `on_join.js` to give
// everyone that's online the challenge.
// 
// Params:
// handle - Challenge handle
function onActivate(handle);

// Called when the challenge is reset
// Params:
// handle - ChallengeHandle for the challenge
function onReset(handle);

```
Although these methods have a `ChallengeHandle` object passed to them via parameters, 
you can access the challenge object or its handle at any time with `_challengeHandle` 
and `_challenge`. Be aware that due to the current scripting system, these fields will 
not be available during initial script evaluation, only after the script is evaluated, 
are they made available