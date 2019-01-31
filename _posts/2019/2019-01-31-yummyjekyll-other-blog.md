# Yummy Jekyll Theme

一个简单的，基于Bootstrap的主题。特别是对于喜欢在网站上展示他们的项目并喜欢做笔记的开发人员。还有一些神奇的功能可供发现。 

## [Live Demo](http://dongchuan.github.io/)

## Notable Features

- 与 Jekyll 3.x and GitHub Pages 相兼容
- 基于 Bootstrap
- [Github Module](http://dongchuan.github.io/open-source) 可以在一个页面和侧边栏上自动显示您的热门项目。（数据由github元数据而不是api调用进行检索，因此没有延迟）
- [Post Module](http://dongchuan.github.io/blog) 用时间轴显示所有文章
- [Bookmark Module](http://dongchuan.github.io/bookmark) 用于建立您喜欢使用的所有库/工具/书籍的快速标记。
- [Post Navigation Module](http://dongchuan.github.io/css/2016/04/22/CSS-Animation.html) 自动根据标题生成导航目录
- Support [Disqus Comment](https://disqus.com/home/explore/)
- Support [Google Analytics](https://analytics.google.com/analytics/web/)

Features in future:

- A Footprint module to show all your travel around the world
- Feature to share. (Facebook, twitter, evernote and so on)
- (Not sure) A embeded todo list. (Not sure) to travel, to complete, to do for your parents, etc. To do in life!
- Creative ideas to discuss with you :P

## Install and setup

在使用它之前，您可能需要在本地安装 [Bower](http://bower.io/) 和 [Bundler](http://bundler.io/) 来安装依赖项.

1. Fork code and clone
2. 运行 `bower install` 去安装 [bower.json](https://github.com/DONGChuan/DONGChuan.github.io/blob/master/bower.json)中的依赖.
3. 运行 `bundle install` 去安装 [Gemfile](https://github.com/DONGChuan/DONGChuan.github.io/blob/master/Gemfile)中的依赖.
4. 修改 `_config.yml` 成自己的配置.
5. 添加文章在 `/_posts`文件夹下
6. 提交代码至 Username.github.io 仓库中.

> 通过bundler或gem安装依赖项时，您可能会遇到一些错误，具体取决于您的环境。

> Error about `json`. Check response of [Massimo Fazzolari on Stackoverflow](http://stackoverflow.com/questions/8100891/the-json-native-gem-requires-installed-build-tools) to quick fix your problem. (Please also use latest version instead of 1.9.3 mentioned in the response)

> Error about `jekyll-paginate`. Please check [here](http://stackoverflow.com/questions/35401566/dont-have-jekyll-paginate-or-one-of-its-dependencies-installed)

> Error about `SSL_connect`. Please check [here](http://stackoverflow.com/questions/15305350/gem-install-fails-with-openssl-failure) and [here](http://railsapps.github.io/openssl-certificate-verify-failed.html)

## How to use

#### Create a new post

将你创建的`.md`文件放入 `_posts` 文件夹.

文件命名遵循 jekyll 格式.

​```
2016-01-19-i-love-yummy.md```

Write the Front Matter and content in the file.

​```
layout: post
title: Post title
category: Category

## tags: [tag1, tag2]

​```

点击 [这里](https://github.com/DONGChuan/DONGChuan.github.io/tree/master/_posts)查看示例

> Jekyll支持不同的存储库结构。您可以在_posts下创建任意数量的文件夹。然后，jekyll将浏览所有文件夹/子文件夹以查找您的帖子。 So cool, right? :D

#### [Post Navigation Module](http://dongchuan.github.io/css/2016/04/22/CSS-Animation.html)

撰写文章时，请始终遵循以下格式：

​```
Description about this post, blablabla

## Title A

### Title A-1

### Title A-2

## Title B

### Title B-1

​```

So, 将检测标题A，A-1，A-2，标题B，B-1并将其创建为目录

For example, [a demo post](https://github.com/DONGChuan/DONGChuan.github.io/edit/master/_posts/2016-04-22-CSS-Animation.md)

但如果你不喜欢它或你的帖子很短。您想要隐藏此导航，以使您的帖子占据整个屏幕。您只需要在要隐藏此功能的帖子的Front Matter中设置**no-post-nav：true**

#### [Github Module](http://dongchuan.github.io/open-source)

该模块将自动从github获取所有存储库信息。但要在当地进行测试，您必须保持互联网连接。将来，它还会显示您贡献的存储库以及您组织的存储库。

#### [Bookmark Module](http://dongchuan.github.io/bookmark)

要添加新标记，您只需编辑 [bookmark.md](https://github.com/DONGChuan/Yummy-Jekyll/blob/master/bookmark.md).

#### [Customize About Page](http://dongchuan.github.io/about)

随意定制about.me页面以显示自己。您只需要修改 [about.md](https://github.com/DONGChuan/Yummy-Jekyll/blob/master/about.md) 和 [about.html](https://github.com/DONGChuan/Yummy-Jekyll/blob/master/_includes/about.html)

## ToDo

- [ ] 按指定标签列出文章
- [ ] New module FootPrint to show your world around trips
- [ ] 在github上显示您组织的项目。(Siderbar, in open-source page)
- [ ] T修复bug - 只能在连接互联网的本地测试。

[教程原文](https://github.com/DONGChuan/Yummy-Jekyll/blob/master/README.md)