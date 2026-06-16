# frontend-docs

前端资料库 —— 基于 VuePress 构建的个人前端知识博客。

## 项目简介

本项目是一个系统性的前端知识库，涵盖了前端开发从基础到进阶的多个领域，包括 JavaScript、CSS、Vue、React、Node、工程化、移动端开发、架构设计等。所有文档均使用 Markdown 编写，方便阅读和维护。

**在线预览**：[https://kitesource.github.io/frontend-docs](https://kitesource.github.io/frontend-docs)

## 技术栈

- [VuePress](https://vuepress.vuejs.org/) v1.7.1 —— 静态网站生成器
- **核心插件**：
  - `@vuepress/plugin-back-to-top`：返回顶部按钮
  - `@vuepress/plugin-medium-zoom`：图片缩放
  - `@vuepress/plugin-pwa`：渐进式 Web 应用支持
  - `vuepress-plugin-reading-progress`：阅读进度条
  - `vuepress-plugin-reading-time`：阅读时长统计
  - `vuepress-plugin-right-anchor`：右侧目录锚点导航

## 内容结构

```
docs/
├── architecture/    # 架构与方案（前端框架、低代码、微前端等）
├── base/            # 前端基础（浏览器、CSS、JavaScript）
├── code/            # 算法与编程
├── devops/          # 工程化（Git、Webpack、Vite、性能优化）
├── mobile/          # 移动端开发（H5、小程序、React Native）
├── react/           # React 全家桶
├── vue/             # Vue 全家桶
└── weekly/          # 前端周刊
```

## 本地开发

### 环境要求

- Node.js >= 14.x
- pnpm（推荐）或 npm

### 安装依赖

```bash
pnpm install
```

### 启动开发服务器

```bash
npm run docs:dev
```

### 构建生产版本

```bash
npm run docs:build
```

构建后的静态文件将输出至 `docs/.vuepress/dist` 目录。

## 部署

项目支持两种方式部署到 GitHub Pages：

**方式一：运行 Shell 脚本**

```bash
bash deploy.sh
```

**方式二：使用 npm 命令**

```bash
npm run deploy:build
```

该命令会先执行 `vuepress build docs` 构建项目，然后通过 `gh-pages` 将构建产物推送到 GitHub 的 `build` 分支。

## 功能特性

- 📖 基于 Markdown 的内容创作
- 📊 阅读进度显示与阅读时间统计
- 🔍 图片缩放、返回顶部等增强体验
- 📌 右侧目录锚点导航
- 🌐 PWA 支持，实现离线访问
- 📱 响应式布局，适配多端阅读

## 贡献

欢迎提交 Issue 或 PR，共同完善前端知识库。

## License

[ISC](LICENSE)