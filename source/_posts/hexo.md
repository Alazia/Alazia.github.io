---
title: Hexo workflow
comments: false
tags: workflow
categories: Hexo
---
##### preparation
- git, add `id_rsa.pub` to 「Deploy keys」
| C:\Users\Administrator\.ssh\id_rsa.pub
- node.js:v12.8.0
- npm (mirror)

```
npm install -g hexo-cli
npm install ## package.json
npm install hexo-deploy-cli@x.x.x
```

##### workflow
```
git clone https://github.com/Alazia/Alazia.github.io.git
hexo new post
hexo clean
hexo g
gulp
hexo d
git add * (and .gitignore)
git commit -m 'source'
git push origin source
```
