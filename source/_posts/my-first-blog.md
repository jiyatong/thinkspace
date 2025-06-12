---
title: 使用 Hexo + NexT 搭建个人博客
date: 2025-06-11 12:00:00
tags:
  - Hexo
  - NexT
  - 博客搭建
categories:
  - 教程
---

# 使用 GitHub Pages + Hexo + NexT 搭建个人博客

本教程将手把手教你如何使用 Hexo 搭配 NexT 主题，在 GitHub Pages 上部署你的个人博客。

---

## 一、环境准备

### 1. Node.js 

### 2. Git

---

## 二、安装 Hexo

使用以下命令安装 Hexo CLI：

```bash
npm install -g hexo-cli
```

---

## 三、创建博客项目

```bash
hexo init my-blog
cd my-blog
npm install
```

启动本地服务：

```bash
hexo server
```

访问 [http://localhost:4000](http://localhost:4000)

---

## 四、安装 NexT 主题

使用Hexo 5.0以上，可以通过npm安装：

```bash
cd my-blog
npm install hexo-theme-next
```

修改 Hexo 主配置文件 `_config.yml`：

```yaml
theme: next
```

---

## 五、个性化 NexT 主题

全局创建 `_config.next.yml`配置文件，并复制基础配置：

```bash
cp node_modules/hexo-theme-next/_config.yml _config.next.yml
```

修改一些基础配置，如：

```yaml
avatar:
  url: /images/avatar.jpg
  rounded: true

menu:
  home: /
  tags: /tags/
  archives: /archives/
```

将头像图片放在 `source/images/avatar.jpg`。

---

## 六、撰写博客文章

在 `source/_posts/` 中创建 Markdown 文件：

```bash
hexo new "我的第一篇博客"
```

编辑 `.md` 文件并保存。

---
