# 内容录入说明

## 目录

| 目录 | 用途 |
|------|------|
| `_posts/` | 长文博客 |
| `_briefs/` | 研究摘要（短文） |
| `_papers/` | 论文条目（链到 PDF/DOI） |
| `_series/` | 系列专题页 |
| `_disclosure/` | 脱敏漏洞披露 |

站点配置：`_config.yml`  
首页简介：`index.md`  
关于页：`about.md`

## 发一篇博客

新建 `_posts/2026-05-20-标题slug.md`（日期前缀必填）：

```yaml
---
title: 文章标题
date: 2026-05-20
categories: [firmware]
tags: [ipc]
series: my-series      # 可选，与 _series 里 series_id 一致
series_order: 1
excerpt: 列表页显示的一句话摘要
---

正文 Markdown。
```

## 其他类型

复制对应目录下的 `example-*` 文件，改名，删掉 `published: false` 后填写内容。

## 系列关联

1. 在 `_series/foo.md` 里写 `series_id: foo`
2. 文章里写 `series: foo` 和 `series_order: 1`

系列页会自动列出该系列下的 posts 与 briefs。

## 暂不发布

```yaml
published: false
```

## 本地预览

```bash
bundle install
bundle exec jekyll serve
```

推送到 GitHub `main` 后由 Pages 自动构建。
