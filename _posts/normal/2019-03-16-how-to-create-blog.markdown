---
layout: post
title:  "使用github pages搭建blog"
date:   2019-03-16 16:03:45 +0800
categories: normal
---
创建Github Repository
修改Settings Repository name为xxx.github.io
修改GitHub Pages Source为Master分支后可以看到blog地址生成

安装Jekyll

``````
sudo apt-get install ruby-full build-essential zlib1g-dev
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
gem install jekyll bundler
``````
创建新的blog

``````
jekyll new myblog
``````
启动Jekyll

``````
bundle exec jekyll serve
启动后127.0.0.1：4000查看
``````
修改_config.yml文件

``````
修改相关数据
baseurl改为github的地址xxx.github.io
重启jekyll可使配置生效
``````
创建blog
``````
在_posts文件下面创建类似模板文件
categories为大类别,会自动在_site下生成和categories的值的同名文件目录
``````

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
