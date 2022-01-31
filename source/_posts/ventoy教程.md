---
title: ventoy教程
date: 2021-09-11 14:48:15
tags: ventoy,U盘
---

**前排提醒**：
多动手搜索，多尝试！
\- [ventoy文档]( https://www.ventoy.net/cn/doc_news.html "ventoy文档") 
\- [百度]( https://www.baidu.com/ "百度")
**所需材料**：
\- 一双灵巧的手 
\- 一个能读字的大脑 
\- 一个U盘 

<!--more-->

# 教程正式开始 
## 1. 下载ventoy并将ventoy安装到U盘中，这一步大多人都会吧 
 ![ventoy]( https://bu.dusays.com/2021/08/30/e3dc893f767cf.png "ventoy") 安装完成后会出现两个盘。 []( http://coolarec.one/wp-content/uploads/2021/08/wp_editor_md_d5a9998f84440ff001519f51d65e3e58.jpg) 
 **请注意，我们的所有操作都是在2盘中进行的** 至此，安装结束，盘中没有任何文件，如果仅仅只是想当做个启动盘用，可以直接传进镜像即可启动 
 附一张官方的截图
[![截图]( https://www.ventoy.net/static/img/screen/screen_bios2.png "截图")]( https://www.ventoy.net/static/img/screen/screen_bios2.png "截图") 


附firpe和微pe获取iso方式 ![]( https://bu.dusays.com/2021/08/30/5179c27657b22.png) ![]( https://bu.dusays.com/2021/08/30/f681a55cf76e8.png) 



## 2. 废话结束，进入正题，美化 想看简洁版教程直接 [点我]( https://www.ventoy.net/cn/plugin_theme.html "点我") 

+ 创建`ventoy`文件夹，并创建`ventoy.json`文件 
+ 下载自己中意的主题文件并传到一个自己能找到到的地方 [下载地址]( https://www.gnome-look.org/browse?cat=109&ord=latest "下载地址") 
+ 按照官方文档在`ventoy.json`中写入 


 >{ "theme": { "file": "/theme/monterey/theme.txt", } } 

其中``/theme/monterey/theme.txt``是主题theme.txt的位置上，``/``表示U盘根目录 
若填入多个file属性，则会随机开启一个主题 ``` "file": [ "/ventoy/theme1/theme.txt", "/ventoy/theme2/theme.txt", "/ventoy/theme3/theme.txt", "/ventoy/theme4/theme.txt" ] ``` 
如果想自定义美化，可根据该theme.txt编辑或替换文件 若过懒的话，可以下载我编辑好的文件，解压并传入U盘根目录 链接见文末 
\## 3. 数据持久化 官方文档：[点我]( https://www.ventoy.net/cn/plugin_persistence.html "点我") 
先上代码
``  "persistence": [ { { "image": "/ISO/ubuntu-20.04-desktop-amd64.iso", "backend": [ "/persistence/ubuntu_20.04_1.dat", "/persistence/ubuntu_20.04_2.dat", "/persistence/ubuntu_20.04_3.dat" ], "autosel": 2 } } ``
将这串代码复制进json文件即可（需要自己修改）
`image`填写镜像位置，`backend`填写对应的文件系统 
至于`autosel`标签，直接上官方文档吧


>可选的，可以不设置。如果设置了之后，在启动前就不会再弹出提示菜单，而是自动选择提示菜单中的对应选项。 
>0: 不使用持久化数据文件 
>1: 使用第1个持久化数据文件 
>2: 使用第2个持久化数据文件 ......



![]( https://bu.dusays.com/2021/08/30/fcbd2591c87d6.png) 
对应文件系统下载地址 

+ [github]( https://github.com/ventoy/backend/releases "github")  
+ [奶牛快传]( https://cowtransfer.com/s/b4e53d5301964e "奶牛快传") 
+  [蓝奏云]( https://wwa.lanzoui.com/iFFe6tcs1hc "蓝奏云") 
  最后是主题文件下载地址 
+ [蓝奏云]( https://wwa.lanzoui.com/iqV0Etcshkb "蓝奏云")   

欢迎大家评论
