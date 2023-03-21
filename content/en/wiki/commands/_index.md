# Syntax
The notation format used to write these command documentations
is similar to [vanilla Minecraft syntax](https://minecraft.fandom.com/wiki/Commands#:~:text=Command%20guide-,Syntax,-In%20Java%20Edition).  
  
We chose to use a slightly different format to provide extra information, 
however. The following command documentation will use this syntax:

| Syntax | Meaning |
|--|--|
| plain text | Requires the literal text to be entered |
| \<argumentName: type> or \<argumentName> | A required argument, the 'type' is not always required, as sometimes it can be inferred by the reader |
| [entry] | A literal value, may optionally be given |
| [\<entry: type>] or [\<entry>] | An argument value, may optionally be given |
| \<first \| second> | (Required) Choose 1 of the literal values |
| [first \| second] | (Optional) Choose 1 of the literal values |

Using the above table as a guide, we can, for example, document the 
`/pay` command like so:
```txt
/pay <players> <amount: number(1..)> [<message>]
```
- `/pay` is the command's label
- `<players>` are the player(s) who will be the target(s) of the command. a 'type' doesn't have to be specified here, as anyone can infer that the command requires us to enter a player's name, or a target selector like `@a`
- `<amount: number(1..)>` The amount of rhines that will be sent to the target(s), here, a type is given for clarity, stating that it requires a number in a range of `[1..]`, aka, above or equal to 1
- `[<message>]` An optional message, like with `<players>` readers can infer that a message is simply any string with color codes or emotes in it.
