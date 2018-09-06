---
layout: post
title:  "jekyll简易教程 -- 1.使用 github pages 和 jekyll 建立博客"
date:   2019-09-05 13:49 UTC+8
categories: jekyll github
permalink: /archivers/jekyll/learn01
---

![github pages]({{ site.url }}/assets/2018-09-05-creat-new-jekyll-blog/github_page.png)

# jekyll简易教程 -- 1.使用 github pages 和 jekyll 建立博客

## 1. 新建 Repository
    该步骤主要为在github上建立新的工程  

![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1536127942_23493.png)

设置`repository name` 为`你的用户名.github.io`  

![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1535958313_31184.png)

Repository name 必需为 `用户名.github.io`

## 2. 设置 Repository
    该步骤主要是将新工程指定为 `github pages`

进入 Repository 页面并点击 Settings  

![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1535958442_32353.png)

查看 `GitHub Pages` 项目  

![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1535958518_25631.png)

先点击 `Choose a theme` 选择任意主题，
`Source` 相关选项通常会自动设置

## 3. 设置 Repository
    该步骤主要是将github上的新工程与本地磁盘上的路径对应

使用 `git` 或 `github disktop` 等方式将主题所在的目录进行同步  
以下以 `github diskto` 为例：

### 3.0 下载安装及登入github账号
具体详细请Goolge

### 3.1 clone repository
![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1536125258_9149.png)

### 3.2 选择 repository 名称和保存位置

![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1536125186_14409.png)

## 4. 下载 jekyll 主题 theme
    该步骤主要是下载jekyll主题

jekyll主题网站：
http://jekyllthemes.org  


注：以下示例以“”主题为例，使用其它主题时可能存在不同。  
https://github.com/laobubu/jekyll-theme-EasyBook  
http://jekyllthemes.org/themes/easybook/  

![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1536126224_32103.png)

在 jekyll主题网站：http://jekyllthemes.org/ 选择合适的主题并下载对应的zip文件
随后将主题解压到git同步目录中。


## 5. 修改 _config.yml
    该步骤主要是配置Blog的基本信息

```yml
# Site settings
title: GRN36909's Blog
# the protocol and hostname of your site, eg. `http://laobubu.github.io`
url: "https://grn36909.github.io"
# the prefix of your site uri, eg. `"/jekyll-theme-EasyBook"` or empty string `""`
baseurl: ""
```

title: blog 名称
url: github pages 链接,通常为 你的用户名.github.io
baseurl: blog路径,通常为空,既""

详细参考：http://jekyllcn.com/docs/configuration/  

## 6. 同步 Repository
    该步骤主要是将本地的主题及修改后的配置提交到github服务器  

进入 github desktop 程序，此时可以看到红色提示的修改信息。  
先在 summary 中输入修改摘要信息,并点击 `Commit to master`提交修改。  
再点击 `Fetch origin` 将修改提交到 github

![]({{ site.url }}/assets/2018-09-05-add_new-articles-to-jekyll/1536125709_19693.png)

## 7. 访问 Blog

使用浏览器访问 `你的用户名.github.io` 即可看到上传的 blog 页面。  
如果未显示 blog 页面，请等待几分钟让 github 完成缓存，
或者清空浏览的`缓存`及`cookies`后再次访问页面。

## 继续阅读

[2.向 jekyll Blog中添加新的文章](https://grn36909.github.io/archivers/jekyll/learn02)

## 本文参考资源

[从零开始折腾Jekyll - 使用Jekyll模板 - biubiu](http://bluebiu.com/blog/learn-to-use-jekyll.html)  

[使用Jekyll + GitHub Pages搭建个人博客 - Xuelong_li](https://www.jianshu.com/p/3caaed303880)  

[Jekyll搭建Github写作环境 - Titan_LEE](https://www.jianshu.com/p/ba240efbfe27)  

[三分钟在GitHub上搭建个人博客 - 天之蓝源](https://zhuanlan.zhihu.com/p/28321740)  

[使用github pages搭建个人免费博客 - Yiweiwoshiniya](https://www.jianshu.com/p/fabb01427203)  

[如何快速搭建自己的github.io博客 - keysaim](https://keysaim.github.io/post/blog/2017-08-15-how-to-setup-your-github-io-blog/)  

[将纯文本转换为静态博客网站 - jekyllcn](http://jekyllcn.com/)  

[如何用github page搭建博客？ - 知乎](https://www.zhihu.com/question/59088760)  

[有哪些简洁明快的 Jekyll 模板？- 知乎](https://www.zhihu.com/question/20223939)  

[我的个人博客之旅：从jekyll到hexo - WordZzzz](https://blog.csdn.net/u011475210/article/details/79023429)  
