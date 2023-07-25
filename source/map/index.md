---
layout: post
seo_title: 开始使用
short_title: 1. 开始使用
author: wanp
group: suode
order: 1
sidebar: [guide, category, suode, toc]
description: Volantis 是一个功能丰富、高度模块化的 Hexo 博客主题。得益于其强大的模块化特性，您可以轻松搭建一个极简风格的博客，也可以仿照官网搭建一个多人协作的、包含文档模块的大体量综合型博客。
---

<p>
{% span logo center large, <sup>&ensp;</sup>Volantis<sup>6</sup> %}
{% span center small logo, A Wonderful Theme for Hexo %}
</p>
<br>

**[Volantis](https://volantis.js.org) 是一个功能丰富、高度模块化的 Hexo 博客主题。得益于其强大的模块化特性，您可以轻松搭建一个极简风格的博客，也可以仿照官网搭建一个多人协作的、包含文档模块的大体量综合型博客。**

{% link 示例博客::/examples/::https://unpkg.com/volantis-static@0.0.1649552113628/media/twemoji/assets/svg/1f433.svg %}

所有的 Volantis 用户都可以按照格式自行创建 [**Issue**](https://github.com/volantis-x/examples/issues/) 来将自己的博客添加到官网的示例博客页面中。

## 准备工作


{% tabs prepare, 1 %}

<!-- tab 能力条件 -->

自建博客需要一定的相关知识，在开始前，请{% u 务必 %}确保您会使用 [markdown](https://www.runoob.com/markdown/md-tutorial.html) 语法，掌握简单的 git 知识，最最重要的是，遇到困难知道该怎么寻求解决：

1. 翻阅和搜索文档
2. 搜索 issues 中是否有解决办法
3. 新建 issue 并按照要求进行操作，详尽地描述您遇到的问题

如果您没有使用过 Hexo 也不要着急，可以先通读一遍 [Hexo](https://hexo.io/zh-cn/docs/) 中文文档，要想使用地得心应手，最好参照团队提供的开源项目的源码进行搭建：

[Demo 源码](https://github.com/volantis-x/demo) ｜ [官网源码](https://github.com/volantis-x/volantis-docs)

<!-- endtab -->

<!-- tab 环境配置条件 -->

如果您从旧版本更新或着其它主题迁移，请确保环境版本不要太低，否则会产生兼容性问题。

```yaml
Hexo: 5.4 ~ 6.x
hexo-cli: 4.3 ~ latest
node.js: 16.x LTS ~ latest LTS
npm: 8.x ~ latest LTS
```

<!-- endtab -->

{% endtabs %}

{% note info :: 配置和使用 volantis 6.x 之前请确保 node.js 升级至 <emp>v16.x 及以上</emp>版本！ %}


{% link FAQ List For Volantis 6::/v6/faq/::https://unpkg.com/volantis-static@0.0.1649552113628/media/twemoji/assets/svg/1fa82.svg %}

## 快速体验

如果您已经具备环境配置条件，可以在终端中输入下面这行代码，稍等片刻即可尝鲜体验：

```bash
git clone https://github.com/volantis-x/demo.git && cd demo && npm i && hexo s
```

related_posts:
        enable: false
        title: 相关文章
        icon: fa-solid fa-bookmark
        max_count: 5
        # 设为空则不使用文章头图
        placeholder_img: https://gcore.jsdelivr.net/gh/MHG-LAB/cron@gh-pages/bing/bing.jpg