---
title: "mail"
linkTitle: "mail"
type: docs
weight: 1
description: >
  mail commands
---


## /mail
Mail command  
  
**Permission**: `ftc.mail`  
**Uses**:
- <pre class="command-usage-arguments">/mail</pre>  
  Mail command  
- <pre class="command-usage-arguments">/mail &lt;page: number(1..)&gt; [&lt;page size: number(5..20)&gt;]</pre>  
  Shows you your mail  
- <pre class="command-usage-arguments">/mail read_other &lt;user&gt;</pre>  
  Reads another user's mail  
- <pre class="command-usage-arguments">/mail read_other &lt;user&gt; [&lt;page: number(1..)&gt;] [&lt;page size: number(5..20)&gt;]</pre>  
  Shows you a users's mail  
- <pre class="command-usage-arguments">/mail send &lt;targets&gt; -anonymous &lt;message&gt;</pre>  
  Sends a mail message to a target player  
- <pre class="command-usage-arguments">/mail send &lt;targets&gt; &lt;message&gt;</pre>  
  Sends a mail message to a target player  
- <pre class="command-usage-arguments">/mail send_item &lt;target&gt; -anonymous &lt;message&gt;</pre>  
  Sends a mail message to a target player with an item  
- <pre class="command-usage-arguments">/mail send_item &lt;target&gt; &lt;message&gt;</pre>  
  Sends a mail message to a target player with an item  
- <pre class="command-usage-arguments">/mail admin_send &lt;targets&gt; [&lt;options&gt;] message=&lt;message&gt;</pre>  
  Sends an admin mail message, options:  
  - [rhines=amount]: Sets the message's rhine rewards  
  - [gems=amount]: Sets the message's gem rewards  
  - [guildExp=amount]: Sets the GuildEXP reward  
  - [items=item list]: Sets the items that are in the message  
  - [script=script name]: Script executed when mail is claimed  
  - [tags=tag list]: Sets a list of string tags used to identify the message  
  - [-multiply-guild-exp]: Sets whether to use the GuildEXP multiplier or not when rewarding GuildEXP  

# Metadata
This is an auto-generated command documentation file generated by the FTC plugin.  
Date: `Sat Nov 18 17:32:09 EET 2023`  
Plugin version: `1.0.0-SNAPSHOT`  
Total commands: 1