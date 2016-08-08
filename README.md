# Creating new posts

In order for Jekyll to realize that a new file is a post (or in this case, a meeting note), the following criteria must be met. 

1. The new document must be placed in the "_posts" folder
2. The file name must follow the pattern yyyy-mm-dd-name.md
3. The contents of the file must begin with the following meta data, **plus an empty line after**:
\--- 
layout: post
title: Monday, January 6, 2014
group: "meeting note"
\---

The title portion can be changed to whatever you would like the meeting note to be titled as, and will be searchable from the meeting notes page. 

The rest of the content is free to be filled in however you choose, but please take note that the site assumes that you are writing your content with [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). To test your markdown before posting it, consider using a live editor like [this one](jbt.github.io/markdown-editor/).
If you prefer to not use markdown, you can use html instead. 