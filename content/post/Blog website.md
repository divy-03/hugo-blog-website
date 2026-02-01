---
title: Blog Website
description: I want my own blog website :)

date: 2025-09-14T20:12:52+08:00
lastmod: 2025-09-14T20:12:52+08:00
tags:
  - blog
  - project
categories:
  - project
---

I also started writing blogs after seeing everyone else's blogs on internet. But to display my blogs I need a website which should render my [[Markdown]]s as content for blogs. 

I can develop a full stack web-app on which one can login write and post blogs, but it requires 3 different servers (frontend, backend, db) and so much efforts if it's only me who is writing the blog. Also I want to use of my already written markdowns. But there is another way instead of developing a full stack website, I can create a static website and push new markdowns every time I write a new blog. Static websites are faster, lighter and much easier to develop.

Planning on using HUGO or might create an own website with use of MDX and NextJs

2025-09-15 
Tags: #hugo #blog 
## Hugo or MDX

After watching few videos on youtube, I decided to use a hugo template.
Found this [Reimu-template](https://github.com/D-Sketon/hugo-reimu-template) the layout is amazing but there are two problems. I'll add Todo's here and write about my progress too in this blog. And later this blog to the website too :)

TODO
- [ ] Remove Chinese from everywhere
- [ ] Replace Images 
- [ ] Add about myself
- [ ] Add my blogs 
- [ ] Change theme colors
- [ ] Deploy on vercel or render
- [ ] Deploy on own domain [[post/How to buy Domain]]
- [ ] Add Japanese (optional)

2025-09-15
Tags: #git #hugo 

### Cloned [Reimu-template](https://github.com/D-Sketon/hugo-reimu-template) and started local server with 
```
git clone https://github.com/D-Sketon/hugo-reimu-template
cd hugo-reimu-template
hugo serve
```

