# sczlzys

## 项目介绍

这是一个基于Hexo框架的个人博客项目，使用Aurora主题，包含了博客文章、分类、标签等功能。

## 项目结构

```
sczlzys/
├── blog/              # Hexo博客主目录
│   ├── source/        # 博客源文件
│   │   ├── _posts/    # 博客文章
│   │   └── page/      # 页面文件
│   ├── themes/        # 博客主题
│   ├── _config.yml    # Hexo配置文件
│   └── package.json   # 项目依赖
├── css/               # 静态CSS文件
├── fonts/             # 字体文件
├── img/               # 图片资源
└── js/                # JavaScript文件
```

## 技术栈

- Hexo 5.4.0
- Node.js
- Aurora主题

## 启动教程

### 1. 环境准备

确保已安装以下软件：
- Node.js (推荐14.x或以上版本)
- npm或yarn

### 2. 安装依赖

进入blog目录并安装依赖：

```bash
cd blog
npm install
```

### 3. 配置修改

根据需要修改`blog/_config.yml`文件：

```yaml
# 网站基本信息
title: Hexo
subtitle: ''
description: ''
author: John Doe
language: en

# URL配置
url: http://example.com/  # 本地启动使用此配置
# url: https://yourusername.github.io  # 部署到GitHub Pages时使用

# 主题配置
theme: aurora  # 使用Aurora主题
```

### 4. 本地启动

执行以下命令启动本地服务器：

```bash
npm run server
```

访问 `http://localhost:4000` 查看博客。

### 5. 构建与部署

#### 构建静态文件

```bash
npm run build
```

静态文件将生成在`blog/public`目录下。

#### 部署（可选）

如果需要部署到GitHub Pages或其他平台，修改`_config.yml`中的部署配置：

```yaml
deploy:
  type: git
  repo: https://github.com/yourusername/yourusername.github.io.git
  branch: gh-pages
```

然后执行部署命令：

```bash
npm run deploy
```

## 常用命令

```bash
npm run clean      # 清理缓存文件
npm run build      # 构建静态文件
npm run server     # 启动本地服务器
npm run deploy     # 部署博客
```

## 主题说明

项目支持以下主题：
- Aurora (默认)
- Landscape
- Sky

可在`_config.yml`中切换主题：

```yaml
theme: aurora  # 切换到Aurora主题
# theme: landscape  # 切换到Landscape主题
# theme: sky  # 切换到Sky主题
```

## 添加文章

使用Hexo命令创建新文章：

```bash
hexo new "文章标题"
```

新文章将生成在`blog/source/_posts/`目录下。

## 自定义配置

更多Hexo配置信息请参考[Hexo官方文档](https://hexo.io/docs/configuration.html)。
