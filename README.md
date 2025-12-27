# Astro 静态博客

一个使用 Astro 构建的最小可执行静态博客示例。

## 快速开始

### 安装依赖

```bash
npm install
```

### 开发模式

```bash
npm run dev
```

访问 `http://localhost:4321` 查看博客。

### 构建生产版本

```bash
npm run build
```

构建后的文件将输出到 `dist/` 目录。

### 预览生产构建

```bash
npm run preview
```

## 项目结构

```
.
├── src/
│   ├── content/          # 博客内容（使用Content Collections）
│   │   ├── blog/         # 博客文章目录
│   │   └── config.ts     # 内容集合配置
│   ├── layouts/          # 布局组件
│   │   └── BlogLayout.astro
│   └── pages/            # 页面路由
│       ├── index.astro   # 主页
│       └── blog/         # 博客文章页面
├── astro.config.mjs      # Astro配置文件
├── package.json
└── tsconfig.json
```

## 添加新文章

1. 在 `src/content/blog/` 目录中创建新的 `.md` 文件
2. 在文件顶部添加frontmatter：

```markdown
---
title: 文章标题
description: 文章描述
pubDate: 2024-01-15
---

你的文章内容...
```

3. 保存文件，Astro会自动生成新的页面

## 特性

- ✅ 使用 Astro Content Collections 管理博客内容
- ✅ 自动生成文章列表和详情页
- ✅ 响应式设计
- ✅ 零JavaScript运行时（默认）
- ✅ TypeScript支持
