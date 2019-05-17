---
title: Hexo搭建博客
date: 2019-05-17 16:27:35
tags:
- hexo
---
![3dfcc383776bc62846294ba96bc6d2f.jpg](https://i.loli.net/2019/05/17/5cde6d91ca1a935726.jpg)

**github新建项目**
项目名使用 username/github.io

**ssh配置**

**安装hexo**
```bash
npm install hexo -g
```

**创建本地目录**
```bash
hexo init blog
```

**新建文章**
```bash
hexo n '文章名'
```

**启动**

本地启动 localhost:4000
```bash
hexo g
hexo s 
```

**安装发布插件**
```bash
npm install hexo-deployer-git --save
```

**修改_config.yml文件**
```bash
deploy:
  type: git
  repository: https://github.com/wenyangliu/wenyangliu.github.io.git
  branch: master
```

**发布**
```bash
hexo clean
hexo g
hexo d
```

**更换主题**
```bash
git clone https://github.com/iissnan/hexo-theme-next themes/next
```

修改_config.yml文件的 theme
```bash
theme: next
```