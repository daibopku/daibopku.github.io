# Bo Dai's Homepage

个人学术主页模板，参考 [yzhu.io](https://yzhu.io/) 设计风格。

🔗 **Live Site**: https://daibopku.github.io

## 设计风格

- **极简学术风格** - 类似 yzhu.io 的清爽设计
- **清晰的层次结构** - Biography → Topics → Pre-Print → Publications
- **响应式布局** - 适配桌面和移动端
- **易于维护** - 模块化内容，方便逐个添加

## 项目结构

```
.
├── _config.yml                # 站点配置（个人信息）
├── _layouts/
│   ├── default.html           # 主页布局
│   └── project.html           # 项目页面布局
├── _projects/                 # 项目集合
│   └── (你的项目文件)
├── _includes/                 # 可复用组件
├── index.md                   # 主页内容
├── projects.html              # 项目列表页
├── Gemfile                    # Ruby 依赖
└── README.md                  # 使用说明
```

## 快速开始

### 1. 配置个人信息

编辑 `_config.yml`：

```yaml
# 基本信息
title: "Bo Dai"
description: "Postdoc in AI at Peking University"

# 个人信息
author:
  name: "Bo Dai"
  email: "your.email@example.com"
  cv: "files/cv.pdf"                    # CV 文件路径（可选）
  google_scholar: "YOUR_SCHOLAR_ID"     # Google Scholar ID（可选）
  github: "your-github-username"        # GitHub 用户名（可选）
  twitter: "your-twitter-handle"        # Twitter 用户名（可选）

# 机构信息
institution: "Beijing Institute for General Artificial Intelligence (BIGAI)"
institution_url: "https://www.bigai.ai/"
advisor: "Prof. Song-Chun Zhu"
advisor_url: "http://www.stat.ucla.edu/~sczhu/"

# 头像（可选，支持外链或本地文件）
avatar: "https://your-photo-url.jpg"
# 或本地文件: "images/avatar.jpg"
```

### 2. 编辑主页内容

编辑 `index.md`，按照以下结构添加内容：

#### Biography 部分
```markdown
<section id="biography">
## Biography

Dr. Bo Dai received a Ph.D. degree ('21) from Peking University advised by [Prof. XXX](链接).
His/Her research focuses on intuitive physics and cognitive science.
Dr. Dai works at [BIGAI](https://www.bigai.ai/), working on Violation of Expectation (VoE) projects.

[<u>CV</u>](files/cv.pdf) [<u>Dissertation</u>](files/dissertation.pdf)
</section>
```

#### Topics 部分
```markdown
<section id="topics">
## Topics

<div class="topics">
  <span class="topic-tag">Intuitive Physics</span>
  <span class="topic-tag">Cognitive Science</span>
  <span class="topic-tag">Machine Learning</span>
</div>
</section>
```

#### Pre-Print 部分
```markdown
<section id="preprints">
## Pre-Print

**Paper Title: Subtitle**
Author One, <u>Bo Dai</u>, Author Three
[<u>arXiv</u>](链接) [<u>Project Page</u>](链接) [<u>Code</u>](链接)

---

**Another Paper Title**
Authors...
[<u>arXiv</u>](链接)
</section>
```

#### Publications 部分
```markdown
<section id="publications">
## Selected Publications

<div class="pub-item">
  <div class="pub-title">Tensor force role in β decays analyzed within the Gogny-interaction shell model</div>
  <div class="pub-authors"><strong>B. Dai</strong>, B. S. Hu, Y. Z. Ma, et al.</div>
  <div class="pub-venue">Physical Review C, 103, 064327 (2021)</div>
  <div class="pub-links">
    [<u>PDF</u>](链接) [<u>DOI</u>](https://doi.org/xxx)
  </div>
</div>
</section>
```

### 3. 添加项目（可选）

在 `_projects/` 文件夹创建新的 `.md` 文件：

```markdown
---
title: "项目名称"
description: "项目简短描述"
date: 2024-01-15
tags: ["标签1", "标签2"]
github: https://github.com/username/repo
paper: https://arxiv.org/abs/xxx
demo: https://demo-link.com
---

## Overview

项目详细介绍...

## Features

- 特性1
- 特性2

## Citation

```bibtex
@article{xxx}
```
```

### 4. 上传 CV 文件（可选）

1. 创建 `files/` 文件夹
2. 上传你的 CV PDF 文件
3. 在 `_config.yml` 中设置 `cv: "files/cv.pdf"`

### 5. 推送更新

```bash
git add .
git commit -m "Update homepage content"
git push origin main
```

GitHub Actions 会自动构建并部署。

## 内容编辑技巧

### 链接格式
- 普通链接：`[文本](URL)`
- 下划线链接：`[<u>文本</u>](URL)` - 类似 [CV] 样式
- 方括号链接：会自动添加 []，如 `[<u>PDF</u>](链接)` 显示为 [<u>PDF</u>]

### 作者名高亮
- 使用 `<strong>Your Name</strong>` 或 `<u>Your Name</u>` 高亮你的名字

### 添加图片
```markdown
![描述](图片URL)
```

### 添加本地文件
1. 将文件放入 `files/` 或 `images/` 文件夹
2. 引用方式：`[CV](files/cv.pdf)` 或 `![头像](images/avatar.jpg)`

## 本地预览

```bash
# 安装依赖
bundle install

# 本地启动
bundle exec jekyll serve

# 访问 http://localhost:4000
```

## 参考网站

- [yzhu.io](https://yzhu.io/) - 设计参考
- [GitHub Pages](https://pages.github.com/) - 托管服务
- [Jekyll](https://jekyllrb.com/) - 静态网站生成器

## 许可证

MIT License
