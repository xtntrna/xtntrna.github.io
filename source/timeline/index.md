---
layout: page
title: 常见问题与反馈渠道
pid: faq
body: [article, comments]
cover: true
sidebar: []
plugins:
  - gitter
---

通常来说，一个全新的工程全部使用默认配置是<green>正常</green>没有故障的。如果无法使用或者效果与示例有较大区别，可以使用 Hexo 官方提供的用于单元测试的博客应用本主题查看样式是否正常，对比 `_config.yml` 文件排查问题。

{% note warning yellow, Hexo 官方的单元测试项目： [https://github.com/hexojs/hexo-theme-unit-test](https://github.com/hexojs/hexo-theme-unit-test) %}

<br>{% btn solid large center, 向开发者反馈问题, https://github.com/volantis-x/hexo-theme-volantis/issues/ , fas fa-paper-plane %}

<!-- more -->

## 如何更新主题

使用主题的时候，尽量 fork 主题到自己的 GitHub，然后进行修改并使用。这样做的好处是：当主题进行重要更新的时候可以根据需要拉取合并代码，使自己 DIY 的主题能够通过更新获取 BUG 修复或者新特性。

如果不懂请自行搜索关键词：<u>fork 更新</u>

{% noteblock idea, 实用小技巧 %}

所有需要写在主题配置文件中的配置都可以写在站点配置文件的 `theme_config:` 中，在 {% u Hexo 5.0 %} 后，还可以写在 `_config.volantis.yml` 文件中，详见 Hexo 官方文档：
{% link 覆盖主题配置::https://hexo.io/zh-cn/docs/configuration#覆盖主题配置::https://unpkg.com/volantis-static@0.0.1649552113628/media/twemoji/assets/svg/1f4da.svg %}

也可以直接查看本站源码中站点配置文件的写法：[_config.volantis.yml](https://github.com/volantis-x/volantis-docs/blob/master/_config.volantis.yml)

{% endnoteblock %}

## 无法成功运行本地预览

- 可能是没有安装依赖，请按照「开始」页面中的步骤进行安装，并安装所需依赖。
- 如果开启了某些第三方服务，请查看文档中是否要求安装插件。
- 如果报错信息有 `lastIndex`，你可以尝试把博客根目录配置文件中找到 `highlight`，并将 `auto_detect` 设置为 `false`。


## 主题配置修改没有生效

请确认文档中要求修改的是博客主目录的配置文件 `blog/_config.yml` 还是主题的配置文件 `blog/_config.volantis.yml`。

## 主题样式修改没有生效

如果主题配置文件中开启了 cdn 服务，那么修改本地的样式是不会生效的，需要关闭 cdn 服务。

## 修改什么都没有生效

需要 `hexo clean` 然后重新 `hexo s`

如果安装了「相关文章推荐」插件后，每次修改 md 文件后都需要重新 `hexo s`

## 关掉 CDN 之后样式错乱

- 请前往文档「开始」页面，检查是否安装了必要的依赖包。
