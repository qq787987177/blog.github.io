---
layout: post
title:  "docker安装"
date:   2019-03-16 20:38:45 +0800
categories: docker
---

安装docker
``````
docker ce
https://docs.docker.com/install/linux/docker-ce/ubuntu/

compose:
https://docs.docker.com/compose/install/

添加Docker用户组，避免总是sudo输入
sudo groupadd docker   #
添加一个新的docker用户组
sudo gpasswd -a username docker   
#添加当前用户到docker用户组里
sudo service docker restart   
#重启Docker后台监护进程
docker version   
#重启之后，尝试一下，是否生效
sudo reboot   
#若还未生效，则系统重启，则生效
docker cmd --help  #
查看命令的详细使用 例如：docker run --help
``````


[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
