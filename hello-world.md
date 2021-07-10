---
title: Hello World
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).
<!-- more -->

## 快速开始

### 创建项目

```bash
hexo new blog
```

### 初始化项目

```bash
hexo init
```

## 自动部署

安装扩展

```bash
npm install hexo-deployer-git
```

配置仓库 `/_config.yml`

```yml
deploy:
  type: 'git'
  repo: 'git@github.com:demodeom/demodeom.github.io'
```

## 下载文章

删除默认文章目录

```language
rm source/_posts
```

克隆文章

```bash
git clone git@github.com:demodeom/hexo-blog.git source/_posts
```
