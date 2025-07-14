# AI News - Jekyll主题（SEO优化版）

一个基于Jekyll的AI新闻博客主题，专注于分享全球AI领域的前沿发展，包括企业动态、产品发布、政策解读等热门AI新闻。

**🎯 2025年全新SEO优化版本**：集成了完整的SEO优化功能，包括智能标签系统、Meta标签优化、文章导航、相关推荐和网站地图等。

## 预览

[Lightfish Blog](http://lightfish.cn)

![Screenshot](https://raw.githubusercontent.com/lightfish-zhang/pinghsu-jekyll/master/preview.png)

![Screenshot](https://raw.githubusercontent.com/lightfish-zhang/pinghsu-jekyll/master/preview2.png)

![Screenshot](https://raw.githubusercontent.com/lightfish-zhang/pinghsu-jekyll/master/preview3.png)

## 🔍 SEO优化功能

### 1. 智能标签系统
- **自动标签提取**：从文章标题和内容中自动提取关键词作为标签（最多5个）
- **标签页面生成**：自动为每个标签创建独立的聚合页面
- **内容链接**：在文章内容中自动为标签相关词汇添加链接
- **支持中英文**：智能识别中英文关键词，支持技术术语识别
- **停用词过滤**：自动过滤常见停用词，确保标签质量

### 2. Meta标签优化
- **Title优化**：自动限制标题长度不超过80个字符
- **Description生成**：自动从文章内容提取前200字符作为描述
- **Keywords生成**：基于文章标签生成关键词（限制100字符）
- **Open Graph**：完整的社交媒体分享优化
- **Twitter Cards**：推特卡片支持
- **作者信息**：自动添加作者meta标签

### 3. 文章导航优化
- **上一篇/下一篇**：文章页面显示导航链接
- **相关文章推荐**：基于标签匹配推荐相关内容（最多10篇）
- **标签展示**：文章页面显示所有相关标签
- **响应式设计**：完美适配移动设备

### 4. 网站地图
- **XML Sitemap**：自动生成符合搜索引擎标准的站点地图
- **包含所有页面**：文章、标签页、静态页面全覆盖
- **Footer链接**：在网站底部添加站点地图链接
- **更新频率**：自动设置不同页面的更新频率和优先级

## 🚀 快速开始

### 配置文件

填写 `_config.yml` 文件：

```yaml
name: Ai news
author: 您的名字
url: https://your-domain.com
baseurl: 
resume_site: https://your-site.com
description: Focus on cutting-edge developments in the global AI field, covering popular AI news such as corporate updates, product launches, and policy interpretations.
github_username: your-username
github: https://github.com/your-username
plugins: [jekyll-paginate, jekyll-simple-search]
permalink: /:year-:month-:day-:title
paginate: 12
paginate_path: "/page/:num/"
exclude: ['README.md', 'Gemfile.lock', 'Gemfile', 'Rakefile']
highlighter: rouge
markdown: kramdown
comments :
  gitalk :
    clientID : xxx
    clientSecret : xxx
    repo : your-repo
    owner : your-username
    admin : your-username
simple_search:
  path:   /search.html
  input_id: search-input
  search_type: json
```

### 文章格式

在 `_posts` 目录下创建文章，格式如下：

```markdown
---
layout: post
title: 文章标题
date: 2025-01-15 00:00:00 +0800
category: 分类名称
thumbnail: /style/image/thumbnail.jpg
icon: book
tags: [标签1, 标签2, 标签3]  # 可选，不设置时会自动提取
---

文章内容...
```

### 标签使用

- **自动标签**：如果不设置tags字段，系统会自动从标题和内容中提取关键词
- **手动标签**：可以手动设置tags数组，推荐3-5个标签
- **标签页面**：每个标签会自动生成独立的聚合页面 `/tags/标签名.html`
- **内容链接**：文章中出现的标签词汇会自动添加链接

## 📝 SEO最佳实践

### 文章优化
1. **标题优化**：控制在80字符以内，包含主要关键词
2. **文章摘要**：在文章开头写一段简洁的摘要（会用作meta description）
3. **标签选择**：选择相关性高的标签，避免过于宽泛
4. **内容质量**：保持文章内容的原创性和专业性
5. **图片优化**：为文章添加缩略图，提高社交分享效果

### 技术优化
- **结构化数据**：文章已包含Schema.org标记
- **移动优化**：响应式设计，完美适配移动设备
- **页面速度**：优化的CSS和JavaScript，快速加载
- **内链建设**：自动为标签词汇添加内链

## 🛠️ 安装部署

### 本地开发

```bash
# 克隆项目
git clone https://github.com/your-username/ainews.git
cd ainews

# 安装依赖
bundle install

# 启动服务
jekyll serve
```

### GitHub Pages部署

1. Fork本项目到你的GitHub账号
2. 在仓库设置中启用GitHub Pages
3. 配置自定义域名（可选）
4. 提交代码自动部署

### 其他平台部署

- **Netlify**：支持自动部署和表单处理
- **Vercel**：快速部署，全球CDN加速
- **AWS S3**：静态网站托管
- **Azure Static Web Apps**：微软云平台部署

## 📊 SEO监控

### 推荐工具

- **Google Search Console**：监控搜索表现
- **Google Analytics**：分析访问数据
- **Google PageSpeed Insights**：页面速度测试
- **SEMrush**：关键词排名监控
- **Ahrefs**：外链分析

### 提交指南

1. **提交sitemap**：将 `/sitemap.xml` 提交给搜索引擎
2. **验证网站**：在各大搜索引擎验证网站所有权
3. **监控收录**：定期检查页面收录情况
4. **优化关键词**：根据数据调整关键词策略

## 📁 项目结构

```
ainews/
├── _config.yml              # 配置文件
├── _includes/               # 页面组件
│   ├── head.html           # SEO优化的头部
│   ├── header.html         # 页面头部
│   ├── footer.html         # 页面底部（含sitemap链接）
│   └── comment.html        # 评论组件
├── _layouts/                # 页面布局
│   ├── default.html        # 默认布局
│   ├── post.html           # 文章页面（含导航和相关文章）
│   └── tag.html            # 标签页面布局
├── _plugins/                # Jekyll插件
│   ├── tag_extractor.rb    # 标签提取插件
│   ├── tag_generator.rb    # 标签页面生成插件
│   └── tag_linker.rb       # 标签链接插件
├── _posts/                  # 文章目录
├── sitemap.xml             # 网站地图
├── style/                  # 样式文件
└── README.md               # 项目说明
```

## 🎨 主题特色

- **响应式设计**：完美适配桌面和移动设备
- **快速加载**：优化的CSS和JavaScript
- **代码高亮**：支持多种编程语言语法高亮
- **搜索功能**：内置文章搜索功能
- **评论系统**：支持Gitalk评论系统
- **SEO友好**：完整的SEO优化方案

## 🔧 自定义配置

### 标签提取配置

标签提取插件支持以下特性：
- 中英文关键词识别
- 技术术语优先识别
- 停用词过滤
- 长度限制（2-15个字符）

可以在 `_plugins/tag_extractor.rb` 中调整：
- 提取的标签数量
- 停用词列表
- 技术词汇词典

### 相关文章配置

可以在 `_layouts/post.html` 中调整：
- 相关文章数量（默认10篇）
- 匹配算法（基于标签交集）
- 显示样式

### Sitemap配置

在 `sitemap.xml` 中可以调整：
- 更新频率设置
- 页面优先级
- 包含/排除特定页面

## 📈 性能优化

### 已实现的优化

- **图片懒加载**：减少初始加载时间
- **CSS压缩**：减少样式文件大小
- **JavaScript优化**：异步加载和压缩
- **CDN加速**：使用CDN加载第三方资源
- **缓存策略**：合理设置缓存头

### 进一步优化建议

1. **图片优化**：使用WebP格式，压缩图片大小
2. **字体优化**：使用web字体，减少加载时间
3. **代码分割**：按需加载JavaScript代码
4. **服务端渲染**：考虑使用SSR提高首屏速度

## 🔄 版本更新

### 2025.01 - SEO优化版本
- ✅ 智能标签系统
- ✅ Meta标签优化
- ✅ 文章导航功能
- ✅ 相关文章推荐
- ✅ XML Sitemap生成
- ✅ 响应式标签页面
- ✅ 内容关键词链接

### 历史版本
- 基础Jekyll主题功能
- 响应式设计
- 代码高亮支持
- 搜索功能集成

## 🤝 贡献指南

欢迎提交Pull Request和Issue！

1. Fork项目
2. 创建功能分支
3. 提交更改
4. 创建Pull Request

## 👥 开发者

- [chakhsu](https://github.com/chakhsu)
- [lightfish-zhang](https://github.com/lightfish-zhang)

## 🙏 致谢

- [jekyll](http://jekyllrb.com) - 静态站点生成器
- [pinghsu](https://github.com/chakhsu/pinghsu) - 原始Typecho主题设计
- [gitalk](https://github.com/gitalk/gitalk) - 基于GitHub Issue的评论系统
- [smoothscroll](https://www.smoothscroll.net/mac/) - 平滑滚动效果

## 📄 许可证

本项目采用MIT许可证，详见LICENSE文件。

## 🆘 支持

如果你在使用过程中遇到问题，可以：

1. 查看本README文档
2. 提交Issue
3. 查看Jekyll官方文档
4. 参考SEO最佳实践指南

---

**享受你的SEO优化之旅！** 🚀
