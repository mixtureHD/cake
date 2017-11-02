# Hexo Configuration
## Docs: http://hexo.io/docs/configuration.html
## Source: https://github.com/hexojs/hexo/

# Site
title: Litten的博客
subtitle: 胆小认生，不易相处
description: 华中科技大学09级，就职于腾讯SNG。擅长各项前端技能，深入研究移动端开发与前端性能。非专业视觉设计师。此为博客一枚。 
author: Litten
email: litten225@qq.com
keywords: "前端,js,jquery,javascript,html5,开发者,程序猿,程序媛,极客,编程,代码,开源,IT网站,Developer,Programmer,Coder,Geek,html,css,css3,用户体验"

# URL
## If your site is put in a subdirectory, set url as 'http://yoursite.com/child' and root as '/child/'
url: //litten.me
root: /
permalink: :year/:month/:day/:title/
tag_dir: tags
archive_dir: archives
category_dir: categories
code_dir: downloads/code
permalink_defaults:

# Directory
source_dir: source
public_dir: public

# Writing
new_post_name: :title.md # File name of new posts
default_layout: post
titlecase: false # Transform title into titlecase
external_link: true # Open external links in new tab
filename_case: 0
render_drafts: false
post_asset_folder: false
relative_link: false
highlight:                                                                                                                                                                                                   
  enable: true                                                                                                                                                                                               
  auto_detect: true                                                                                                                                                                                          
  line_number: true                                                                                                                                                                                          
  tab_replace: ''

# Category & Tag
default_category: uncategorized
category_map:
tag_map:

# Archives
## 2: Enable pagination
## 1: Disable pagination
## 0: Fully Disable
archive: 1
category: 1
tag: 1

# Server
## Hexo uses Connect as a server
## You can customize the logger format as defined in
## http://www.senchalabs.org/connect/logger.html
port: 4000
server_ip: localhost
logger: false
logger_format: dev

# Date / Time format
## Hexo uses Moment.js to parse and display date
## You can customize the date format as defined in
## http://momentjs.com/docs/#/displaying/format/
date_format: YYYY-MM-DD
time_format: HH:mm:ss

# Pagination
## Set per_page to 0 to disable pagination
per_page: 8
pagination_dir: page

# Disqus
disqus_shortname:

# Extensions
## Plugins: https://github.com/hexojs/hexo/wiki/Plugins
## Themes: https://github.com/hexojs/hexo/wiki/Themes
# plugins:
#  - hexo-generator-feed
#  - hexo-generator-baidu-sitemap
#  - hexo-generator-sitemap

theme: yilia
exclude_generator:

# Deployment
## Docs: http://hexo.io/docs/deployment.html
#deploy:
#  type: git
#  repository: git@github.com:litten/litten.github.com.git
#  branch: master

deploy:
  type: rsync
  host: 120.24.181.238
  user: root
  root: /usr/local/nginx/litten.me/
  port: 22

sitemap:
    path: sitemap.xml
baidusitemap:
    path: baidusitemap.xm

feed:
    type: atom
    path: atom.xml
    limit: 100

jsonContent:
  meta: false
  pages: false
  posts:
    title: true
    date: true
    path: true
    text: false
    raw: false
    content: false
    slug: false
    updated: false
    comments: false
    link: false
    permalink: false
    excerpt: false
    categories: false
    tags: true