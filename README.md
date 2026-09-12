# 合租生活管家

面向年轻合租人群的交互式产品雏形，包含费用 AA、清洁值日、公共物品和室友公约四个模块。

## 技术形态

- 零依赖静态站点，仅使用 HTML、CSS 和原生 JavaScript。
- 无需服务端、数据库或构建工具。
- 示例数据随页面提供，操作结果保存在当前浏览器的 `localStorage` 中。
- 适合直接部署到 GitHub Pages。

## 固定生产地址

仓库必须命名为 `<你的 GitHub 用户名>.github.io`，并保持公开。部署成功后，生产地址为：

```text
https://<你的 GitHub 用户名>.github.io/
```

后续只需继续向 `main` 分支提交代码，GitHub Actions 会更新同一个生产地址。

## 自动部署

工作流文件位于 `.github/workflows/deploy-pages.yml`，会在以下情况运行：

- 代码推送到 `main` 分支；
- 在 GitHub Actions 页面手动运行。

首次部署前，需要在仓库的 `Settings → Pages → Build and deployment` 中将 `Source` 设置为 `GitHub Actions`。
