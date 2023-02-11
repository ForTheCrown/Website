---
title: "Running Scripts"
linkTitle: "Running Scripts"
weight: 1
description: >
  Everything related to running scripts.
---

{{% pageinfo %}}
Running scripts can be done by Commands or from Java code.
{{% /pageinfo %}}

## By Command
```
/scripts run <script name> [<function name>]
```
- `<script name>` - The script's file path within the `scripts` directory, you can use tab completions to find the one you're lookingfor.  
- `[function name]` - An optional argument for the name of the function within the script to call.  
    
You can also execute raw JavaScript code by using the `eval` command 
like so:
```
/scripts eval <java script code>
```

### Examples:
`/scripts run path/to/script.js`  
Simply runs the script file, not calling any methods

`/scripts run path/to/script.js methodName`  
Evaluates the script file like above, and after executes The method 
named 'methodName'

`/scripts eval let x = 0; let y = 1; print(x + y);`  
Executes the raw JavaScript code that's passed to it

## From Java code
First, we'll need to create an instance of the `Script` class, we can do
so using one of the following methods:  
  
Via a file path:
```java
import net.fothecrown.core.script2.*;

Path path = /* Acquire it somehow */
Script script = Script.of(path);

// This string path is relative to the `plugins/ForTheCrown/scripts`
// directory
String stringPath = /* Create a path */
Script anotherScript = Script.of(stringPath);
```
Or via raw JavaScript:
```java
String jsCode = "print('Hello, world!')";
Script script = Script.ofCode(jsCode);
```
Next, we'll need to compile and then evaluate the script
```java
Script script = // ...;

// This will load and compile the script
script.compile();

// After compilation, you can place any optional binding
// values into the script, these will be accesible from
// inside the script
script.put("a_binding_value", "Foor");

// Evaluate the script's main function, aka run it
// Returns a result detailing how the execution went.
ScriptResult result = script.eval();

// Test if the execution failed due to an error
// Note: If any error was thrown, it will be logged automatically
if (result.error().isPresent()) {
  return;
}

// result() returns an Optional<Object>, empty if there was an
// error, or if the function returned nothing
Object resultingObject = result.result().orElse(null);

// This will return the resultingObject, shown above, as an
// Optional<Boolean>. If the resultingObject doesn't exist, or
// can't be converted to a boolean, this method returns empty
result.asBoolean();
```