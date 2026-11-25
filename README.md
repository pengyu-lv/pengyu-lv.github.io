# mypage

一个纯静态博客，托管在 GitHub Pages。自带一套手写的设计系统（衬线标题 + 纸感配色 + 深色模式），不依赖第三方主题。

- 写文章 = 在 `_posts/` 里加一个 Markdown 文件
- 推送后 GitHub 自动构建，1~3 分钟上线
- 本机不需要安装任何东西

## 三步上线

1. 改 `_config.yml` 里标了【必改】的 3 处
2. 把整个文件夹推到 GitHub 仓库
3. 仓库 Settings → Pages → Source 选 `Deploy from a branch` → `main` + `/(root)` → Save

详细步骤见 **[配置指南.md](配置指南.md)**。

## 目录

| 文件 | 作用 |
|---|---|
| `_config.yml` | 站点配置，唯一必改的文件 |
| `index.md` | 首页（用 `home` 布局） |
| `about.md` | 关于页 |
| `404.html` | 404 页面 |
| `_posts/` | 文章目录 |
| `_layouts/default.html` | 页面骨架：顶栏 + 正文 + 页脚 |
| `_layouts/home.html` | 首页：大标题 + 文章卡片列表 |
| `_layouts/post.html` | 文章页：元信息 + 正文 + 上下篇 + 评论 |
| `_layouts/page.html` | 普通页面（关于、404） |
| `_includes/head.html` | `<head>`、SEO、深浅色初始化 |
| `_includes/header.html` | 吸顶导航栏 + 主题切换按钮 |
| `_includes/footer.html` | 页脚 |
| `_includes/comments.html` | giscus 评论框 |
| `assets/main.scss` | 全部样式（设计变量都在文件开头） |

## 想改样子

打开 `assets/main.scss`，文件最上面的 `@mixin theme-light` / `theme-dark` 里就是全部配色：

```scss
--accent: #b04a1f;   /* 主色，标题竖线、链接、标签都是它 */
--bg: #faf9f6;       /* 背景 */
--text: #1b1b19;     /* 正文颜色 */
--font-serif: ...    /* 标题字体 */
```

改一个变量，全站跟着变。
