---
title: "Java Interopability"
linkTitle: "Java Interopability"
weight: 2
description: >
  Everything related to java.
---

{{% pageinfo %}}
The JavaScript engine used by FTC (Nashorn) is completely compatible with Java.
{{% /pageinfo %}}

The JavaScript engine used by FTC (Nashorn) is completely compatible 
with Java.
  
To this end, you can import java classes like almost just like you would
in regular Java, for example, to import the [Time utility class](https://github.com/ForTheCrown/FTC/blob/main/src/main/java/net/forthecrown/utils/Time.java), you can use the following:
```js
import "@ftc.utils.Time";
```
The `@ftc` is an 'import placeholder', basically used to make import 
statements shorter and less of a hassel to write. All import 
placeholders are defined in [`import_placeholders.toml`](https://github.com/ForTheCrown/FTC/blob/main/src/main/resources/scripts/import_placeholders.toml)  
  
If you're encountering issues with the above shown method, you can 
fallback to Nashorn's actual method of importing classes:
```js
const Time = Java.type("net.forthecrown.utils.Time");
```
FYI, the method of using the 'import' keyword, is just remapped to the second method
by a preprocessor, thus, in effect, the 2 above methods are essentially the same
  
Please also be aware that the Nashorn engine, is not 100% up to ECMAscript 6 standards,
there are many missing features. Be careful when using newer JavaScript features such as
classes, as they do not exist within the engine.

## Built in
The script engine comes with several custom built in parts, the 
first of these are the classes that are automatically imported in to every script.  
Be aware, this list may not be complete, see the [BuiltIn class](https://github.com/ForTheCrown/FTC/blob/main/src/main/java/net/forthecrown/core/script2/ScriptsBuiltIn.java) for the definitive list of all imported classes.  
- `org.bukkit.Bukkit`
- `org.bukkit.Location`
- `org.bukkit.enity.EntityType`
- `org.bukkit.Material`
- `net.kyori.adventure.text.Component`
- `net.kyori.adventure.text.format.NamedTextColor`
- `net.kyori.adventure.text.event.ClickEvent`
- `net.kyori.adventure.text.event.HoverEvent`
- `net.kyori.adventure.text.format.Style`
- `net.kyori.adventure.text.format.TextDecoration`
- `net.forthecrown.utils.text.Text`
- `net.forthecrown.utils.Util`
- `net.forthecrown.utils.Cooldowns`
- `net.forthecrown.utils.inventory.ItemStacks`
- `net.forthecrown.utils.math.Bounds3i`
- `net.forthecrown.utils.math.WorldVec3i`
- `net.forthecrown.utils.math.WorldBounds3i`
- `net.forthecrown.utils.math.Vectors`
- `net.forthecrown.user.Users`

Ontop of these imports, you are given a `Log4J` logger to use for 
logging, accessible like so:
```js
logger.info("I am logged message! :)");
```
###### Note: Any logger calls on level `ERROR` will be automatically forwarded to the `error-log` channel in Discord.
  
And a function to compile other scripts:
```js
// This will only perform the Script#compile() call
// Note: the path given to this function is relative to
//  file of the current script
const otherScript = compile("path/to/script.js");

// Here, just like above, you can place objects into the script's
// bindings, but in a simpler way, like so:
otherScript.foo = "bar";

// calls Script#eval()
// Will throw an exception if the script's evaluation fails and
// returns the result of the script's evaluation
let result = otherScript();
```