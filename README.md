semitransparent-jekyll-theme
===============================

[semitransparent-wordpress-theme](https://github.com/zeruniverse/semitransparent-wordpress-theme)的Jekyll实现。借鉴了[theme-hushaw](https://github.com/jekyllrc/theme-hushaw)

## Demo

本项目的GitHub [Pages](https://zeruniverse.github.io/semitransparent-jekyll-theme/)

## Features

+ 半透明风格

+ 中文支持

+ RSS支持

+ 动态背景

+ 仿WordPress

+ 分页支持

+ 配图支持

+ 首页显示摘要

## Installation

[安装Jekyll环境](https://jekyllrb.com/docs/installation/)，然后下载本项目。如果您希望在GitHub上搭建博客，只需要Fork这个项目，修改`_config.yml`，然后把博文放进`_post`文件夹。

## Front Matter

+ layout请设置成post

+ hgimg: 文章配图（可选项），您需要将图片放进`postimg`文件夹然后在这里指定文件名。

+ fullhgimg: 高清版配图（可选项，只在hgimg已指定的情况下有效），您需要将图片放进`postimg`文件夹然后在这里指定文件名。

+ 其它设置请参见Jekyll文档

+ 请在文章合适的地方加上`<!--more-->`。之前所有内容将被作为摘要。请尽量在每篇文章中都设置`<!--more-->`，否则首页会太长。

## Customerization

+ 页面上方图片支持随机从图库中选择。图片数量由`_config.yml`中的`hgimgcount`控制。图库的位置是`/static/hgimg`，里面必须放1000*288的jpg图片，图片需命名为`1.jpg 2.jpg ...`。

+ 您可以创建自定义页面，请参考`about.html`。

+ 您可以定制首页右侧的相关链接，修改`_config.yml`中的`navigation`变量。

## Issues

+ GitHub Pages 判断变量是否为空的函数有问题，Jekyll没有remove_last这个filter，因此这两个地方用了比较奇怪的实现方式。

+ 同款WordPress的气泡背景加到这里会导致浏览器卡死。原因未知，因此换了雪花背景。

## License

GNU GPU v3. The copyrights of all libraries are reserved by their authors.