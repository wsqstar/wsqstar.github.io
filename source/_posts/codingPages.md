---
title: codingPages
date: 2020-01-20 20:36:48
tags:
- Github
- BLOG
---
Pages服务是目前实现个人博客的一种方式。
Coding.net 在2020年初大版本更新之后也给我们带来了更加优异的体验。
正好也上了双线Pages服务，使用阿里云DNS解析，免费、快速、智能。
现在只有域名是托管在Gandi上面，DNS是阿里云的，页面是同时推送到Github以及CodingPages上面。
emmm，有点遗憾的是，目前的备份不太好用QAQ。
同时很惊讶的发现——似乎文件更新缓慢？？？

## 20200126
在群里问大家网页不显示最新文件的问题，
热心群友， https://ntaurus.com/ ，建议：

1.换cmd里已绑定的coding仓库地址
2.把文件推上coding
3.在coding的静态网站里点->立即部署
4.在域名管理添加CNAME指向coding给的访问地址
5. 静态网址设置里绑定自定义域名
6.添加TXT记录指向->步骤5绑定时给的 记录值（字符串）
(！！部署前先停用指向github的解析)


另外，目前为了稳定，暂时仅仅开启了coding的DNS解析。

顺便尝试了https上传，不用不安全的ssh
可以这样来：

git remote add origin https：（github添加仓库）
git remote set-url --add origin xxx	(添加coding仓库)
再敲这个添加

但是我是这样做的：

直接更换地址，会弹出一个登录框，登录即可。