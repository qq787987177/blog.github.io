---
layout: post
title:  "docker nginx 启动失败"
date:   2019-03-16 20:38:45 +0800
categories: docker
---
docker nginx 启动失败
``````
开机时 apache2 自动启动，占用了80端口。

解决方法：

service apache2 stop
``````


[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
