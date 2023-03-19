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

This means you can import java classes, instantiate them, or use their static
methods like you would normally in Java.

## Importing java classes
In this example, we'll import the `java.lang.System` class to print something
to the console:
```js
import "java.lang.System";
System.out.println("Hello, world!");
```
We can also give an alias to our imports like so:
```js
import * as AliasedSystem from "java.lang.System";
AliasedSystem.out.println("Hello, aliased world!");
```
### Import placeholders
Import placeholders are a little tool to make writing import statements less of
a hassel. All placeholders are defined in [`import_placeholders.toml`](https://github.com/ForTheCrown/FTC/blob/main/src/main/resources/scripts/import_placeholders.toml).
  
As an example, we'll import the same java system class, but with imports
```js
import "@jlang.System";
System.out.println("Hello, placeholder-ed world!");
```
## Importing other scripts
While Nashsorn does not support CommonJS modules... or modules at all, FTC's
scripts do allow for you to import other scripts using the following technique:
```js
// Imports and compiles the script
import "path/to/script.js";
// Evaluates the script's global scope
script(); 

script.a_method();
```
The same aliased import statement also works for these imports:
```js
import * as aliasedScript from "script/path.js";
aliasedScript()

aliasedScript.method();
```
**Note**: These import statements are very limited, you cannot import specific
methods from individual scripts like with `import { m_1, m_2 } from "foo/bar.js"`.

###### Praying that some day Java will have JavaScript engine that isn't 9 years behind

### Behind the scenes
Behind the scenes, both of the above-shown imports are ran through a JS Preprocessor that translates those import statements to JS code. For example, the following import `import "@ftc.core.Worlds";` is translated into `const Worlds = Java.type("net.forthecrown.core.Worlds");`.
  
Script imports are translated from `import "path/to/script.js"` to `const script = compile("path/to/script.js");`
  
Using the `as` keyword in imports simply changes the name of the `const` value
  
So, if you're having problems with using import statements, feel free to 
fallback to those method calls. Be aware, neither of those 2 methods support the
import placeholders however.

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
