---
layout: post
title:  "Docker 容器中安装composer"
date:   2019-03-23 12:38:45 +0800
categories: docker
---

安装composer
``````
1.下载composer.phar

wget https://getcomposer.org/composer.phar

2.重命名composer.phar为composer

mv composer.phar composer

3.将composer放入容器中

docker cp composer php:/usr/local/bin

4.增加可执行权限

docker exec -it php bash
cd /usr/local/bin
chmod +x composer

5.查看是否成功

composer
``````


[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
