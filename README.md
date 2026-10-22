# 个人博客

这个站点基于 [AstroPaper](https://github.com/satnaing/astro-paper) 搭建，使用 Astro 静态生成并部署到 GitHub Pages。

## 本地运行

需要 Node.js 24 和 pnpm 11。

```sh
pnpm install
pnpm dev
```

## 发布文章

在 `src/content/posts/` 新建 Markdown 或 MDX 文件。文章需包含标题、发布日期和简介，例如：

```yaml
---
title: "文章标题"
pubDatetime: 2026-10-22T00:00:00Z
description: "文章简介"
---
正文从这里开始。
```

## 部署

推送到 `main` 后，GitHub Actions 会构建并发布到 GitHub Pages。仓库 Pages 来源需设为 **GitHub Actions**。站点使用项目路径 `/astro-paper-blog`。
