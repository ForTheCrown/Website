## Information

These files are used to create the static pages of www.forthecrown.net. 

To generate the static files, I use [Hugo](https://gohugo.io/). And to set something up quickly, I've picked a theme called [Docsy](https://www.docsy.dev/).

Once the static pages are generated, they can be uploaded to [this public repository](https://github.com/ForTheWout/ForTheWout.github.io). 
This repo uses Github as a webhost, mainly because it's free. [Here](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages) you can find more info if want to know more about how that works.  
The website itself can be updated by changing the files in that public repository that hosts the page. 

## Contributing

You can make changes to the wiki pages by editing the markdown files in [content/en/](content/en/). 
The [wiki](content/en/wiki/) folder is for the player wiki, the [docs](content/en/docs/) folder is for the dev wiki.

To make a new section, make a new folder with an _index.md file inside. Hugo uses some special syntax, I find it easiest to copy an existing file and edit it.

For an example of how the file structure works, see the dev pages about [challenges](/content/en/docs/Challenges/) or [scripts](/content/en/docs/Scripts/).

## Idea Dumpster 

Here is a place to store ideas of what would be cool to have on the website.

- Create a dark theme option.
- Add a community section to highlight builds made on server.
- Make a page for guilds on the server, like `/g discover` in-game.
- Make homepage background scroll through images of the server instead of being static.
