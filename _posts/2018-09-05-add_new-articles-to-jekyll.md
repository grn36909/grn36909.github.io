---
layout: post
title:  "jekyll简易教程 -- 2.向 jekyll blog中添加新的文章"
date:   2019-09-05 19:25 UTC+8
categories: jekyll
permalink: /archivers/jekyll/learn02
---

![jekyll]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/jekyll.jpg)

# jekyll简易教程 -- 2.向 jekyll blog中添加新的文章

## 1. jekyll Blog 目录结构

参考：http://jekyllcn.com/docs/structure/  

本地磁盘和 github 上的 jekyll 工程目录的文件结构应该为如下格式：

```
.
├── _config.yml
├── _drafts
|  ├── begin-with-the-crazy-ideas.textile
|  └── on-simplicity-in-technology.markdown
├── _includes
|  ├── footer.html
|  └── header.html
├── _layouts
|  ├── default.html
|  └── post.html
├── _posts
|  ├── 2007-10-29-why-every-programmer-should-play-nethack.textile
|  └── 2009-04-26-barcamp-boston-4-roundup.textile
├── _site
├── .jekyll-metadata
└── index.html
```

- 通常用户文章应存放在 `_posts` 文件夹中

## 2. jekyll Blog 文章格式要求

- 文件格式为 `MarkDown`
- 文件名格式为 `YYYY-MM-DD-文件名.md`

`YYYY` 为年份，4字符  
`MM` 为月份，2字符  
`DD` 为日期，2字符  

具体的 `MarkDown` 文件书写规范请自行 `Google`

## 3. 添加头信息到文件

详细参考：http://jekyllcn.com/docs/frontmatter/  

添加头信息到文件的最前面
```
---
layout: post
title:  "向 jekyll Blog中添加新的文章"
date:   2019-09-05 19:25 UTC+8
categories: jekyll
permalink: /archivers/jekyll/learn02
---
```

- layout： 指定文章所使用的模板
- title：指定文章的标题
- date：（可选）指定文章的日期，该设置优先于文件的日期属性
- categories：（可选）指定文章的分类
- permalink：（可选）指定文章的永久链接（短链接）

## 4. 上传文章 到 jekyll Blog

用户在本地磁盘中编写 `MarkDown` 格式的文件，并保存为 `YYYY-MM-DD-文件名.md` 格式的文件名。
将文件复制到本地磁盘的 `_posts` 文件夹中，并通过 `git` 或 `github desktop` 程序同步到 `github` 端

## 5. 查看文章

通过浏览器访问 github pages 地址

## 前文回顾

[1.使用 github pages 和 jekyll 建立博客](https://grn36909.github.io/archivers/jekyll/learn01)  

## 继续阅读

[3.Markdown 指南](https://grn36909.github.io/archivers/jekyll/learn03)
