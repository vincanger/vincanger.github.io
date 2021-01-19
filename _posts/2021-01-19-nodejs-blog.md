---
title: "Markdown NodeJS Blog Generator"
date: 2021-01-19
tags: [NodeJS, ExpressJS, Javascript, markdown, repl.it]
excerpt: "Simple, static blog generator made with NodeJS"
---

### My objectives:
- Create my own blog using NodeJS ✅
- Learn `fs` commands in NodeJS ✅
- Convert Markdown files to HTML using the `marked` module ✅
- Create an Express server and host it on repl.it ✅
  - https://blog.vincanger.repl.co
- ✌

### How the code works:
- Posts are made as individual MD files (see 'content' folder)
- Front-matter within the posts gets parsed
- The `marked` module converts MD to HTML
- and the magic of JavaScript puts it all together 🧙‍♂️

```JavaScript
const createPost = postPath => {
  const data = fs.readFileSync(`${config.dev.postsdir}/${postPath}.md`, "utf8");
  const content = fm(data);
  content.body = marked(content.body);
  content.path = postPath;
  return content;
};
```