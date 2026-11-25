---
layout: post
title: "第一篇：这个博客是怎么搭起来的"
date: 2026-11-25 10:00:00 +0800
tags: [随笔, GitHub Pages]
---

这是一篇示例文章，可以整篇删掉，换成你自己的内容。

## 怎么写新文章

在 `_posts/` 目录下新建一个文件，**文件名必须是 `年-月-日-英文标题.md`**，例如：

```
_posts/2026-12-01-my-first-post.md
```

文件开头必须有 front matter：

```yaml
---
layout: post
title: "文章标题"
date: 2026-12-01 09:00:00 +0800
tags: [标签一, 标签二]
---
```

下面的正文就是普通的 Markdown。

## 支持的写法

**加粗**、*斜体*、`行内代码`、[链接](https://pages.github.com)。

> 引用块。

- 无序列表
- 第二项

1. 有序列表
2. 第二项

```python
def hello(name):
    print(f"你好，{name}")
```

表格：

| 功能 | 是否支持 |
|---|---|
| Markdown | ✅ |
| 代码高亮 | ✅ |
| 评论 | ✅（配好 giscus 后） |
| 数学公式 | ❌ 需要额外插件 |

图片放在仓库任意位置，用相对路径引用即可：

```markdown
![示意图](/assets/images/demo.png)
```

## 发布

提交并推送后，GitHub Actions 会自动构建，大约 1 分钟后线上就能看到。
