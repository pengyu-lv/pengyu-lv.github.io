# mypage

一个用 Jekyll + minima + giscus 搭的静态博客，托管在 GitHub Pages。

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
| `index.md` | 首页，自动列出全部文章 |
| `about.md` | 关于页 |
| `404.html` | 404 页面 |
| `_posts/` | 文章目录 |
| `_layouts/post.html` | 文章页模板 |
| `_includes/comments.html` | 评论框 |
| `assets/main.scss` | 自定义样式 |
