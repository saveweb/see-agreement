---
title: 主页
date: 2022-01-21 14:43:41
---

这是收录网络服务或者软件的服务条款的网站，包括但不限于用户协议、隐私协议等。

使用了 MkDocs ([Material for MkDocs][]) 来生成静态页面。

[Material for MkDocs]: https://squidfunk.github.io/mkdocs-material/

## 收录方式

1.  获取服务条款

    服务条款通常是具体的 URL，这很容易收录，但部分 APP 的服务条款可能会有意无意的隐藏服务条款的 URL，这时通常只能直接复制内容了，如果无法复制，那么可能需要使用 Universal Copy 这样的，能够从 UI 框架里提取文字内容的工具。

2.  记录元数据

    see-agreement 的目标不仅仅是保存服务条款的全文，还要记录以下元数据记录：

    +   添加时间
    +   最后可见时间
    +   URL
    +   Internet Archive 链接

    如果没有 URL，那么截图之类的资料也许要留存。

3.  展示条款

    MkDocs 使用的 Markdown 渲染器是 [Python-Markdown][]，这个渲染器能启用或者停用各种不同的 Markdown 扩展功能，所以如果遇到渲染问题，也许可以检查仓库根目录的 mkdocs.yml 文件的 markdown_extensions 部分，确认目前配置文件所支持的扩展功能。

    此网页有使用 i18n 插件，所以能够支持同一个页面的多语版本。

    如果条款的排版格式过于复杂（比如多级标题和粗体），那么 see-agreement 会在文本头部留下「忽略排版提示」，告知此页面的排版没有按照原样呈现。

[Python-Markdown]: https://python-markdown.github.io

## 参与方式

在仓库的 [Issues](https://github.com/saveweb/see-agreement/issues) 页面创建一个含有服务条款名称和 URL 的页面，这就是推荐的参与 see-agreement 建设的方式，也可以在 Telegram 的 [Save The Web \[Chat\]](https://t.me/saveweb_chat) 群组里提交。

掌握 MkDocs 和 Python-Markdown 可能稍微需要一些时间，所以如果不是深度参与 see-agreement，或者使用 MkDocs，那么没有必要为此花费时间，文本整理等后续工作交给 Save The Web 的 MkDocs 小组就好。
