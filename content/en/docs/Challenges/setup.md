---
title: "Setup"
linkTitle: "Setup"
weight: 1
description: >
  The `plugins/ForTheCrown/challenges/challenges.json` file is where all challenges are loaded from.
---

{{% pageinfo %}}
This section documents the format the `challenges.json` file uses to read challenges.
{{% /pageinfo %}}



  
First of all, it's a JSON object file, where each entry's key is the ID they will be registered with and where the values are the challenge data. The following is a list of valid keys for challenge data, optional entries will have an `*` after their name.  
  
Some of the possible values accepted in the challenges json are based on 'streak-based values', which means they can dynamically change for each users based on their current streak for the challenge in question.  
  
Accepted inputs for streak-based values are:  
**Fixed value**  
The returned value is a constant which doesn't change
```json
"rhines": 200
```
**Scalar-based value**  
Which calculates the reward value like so: `reward = base * (streak * scalar)`.
Normally, a player's streak begins at 0, however, to ensure this value stays 
functional, if the given streak is 0, it is incremented to 1.
```json
"rhines": { "base": 200, "scalar": 0.5 }
```
**Array-based value**

These will get the value by treating a user's streak as an index to an array of rewards, if a user's streak is higher than the array size,
the index is clamped and the final reward is used. In the following example, a streak of 0 days would return 200, a streak of 1 day
would return 400 and so on
```json
"rhines": [ 200, 300, 400, 600, 1200 ]
```
  
---
### `displayName`
This is the name that's used to display the challenge to users in chat and the challenge book.
This can be either a string or a more complex Chat Component.
  
---
### `description`*
An array of elements that's used as a description of the challenge, displayed in the `displayName` hover event. As such, it's accepted input is similar to `displayName`. If no value is set for this, then the description will simply be empty.
  
---
### `reward`*
Specifies data of rewards given to a user when they complete the challenge, accepts the following entries:
- `guildExp`: The amount of guildExp given to users that complete the challenge, if user is not a guild, no exp is given (streak-based).
- `rhines`: Rhine reward given to the player (streak-based).
- `gems`: Gem reward given to the player (streak-based).
- `item`: Item given to the player upon completion.
- `claimScript`: The script called when a player claims the reward, the system will call the `onRewardClaim` method with the user as the parameter

If no value is set for this, then no reward will be given.
  
---
### `goal`*
A streak-based value specifying how many points are required to complete a challenge, If no goal is set, it defaults to `1`
  
---
### `type`*
Specifies the frequency at which the challenge is reset, accepts one of the following inputs:
- `daily`: Challenge is reset once a day
- `weekly`: Challenge is reset every monday
- `manual`: Challenge will not be selected nor reset by itself, requires code or staff input to make this challenge active.

If no value is specified, then this defaults to `daily`  
  
---
### `script`*
The filename of the script responsible for handling the challenge logic.
Examples of valid input:
- `script_name.js`
- `directory/script_name.js`

If this value is not set, no script is used. See the Scripts section for more info on scripts.
  
---
### `eventClass`
The fully qualified class name of the event this challenge listens for.  
If no script is given, then this class must be a sub-class of `PlayerEvent`, otherwise, the challenge handler will not be able to get the player from the event.  
  
If a script is given, but no event handling method is specified AND the event is not a sub-class of `PlayerEvent`, then this system requires that the script specifies a `getPlayer` method which takes the event as input and returns the event's player object.  
  
If this value is unset or left as `"custom"`, then this challenge will never be called from an in-game event, and will instead require to be manually triggered by FTC's plugin.