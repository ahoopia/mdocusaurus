---
title: Linux motd 欢迎信息配置
tags: [工具,Linux]
---



今天登录VPS的时候发现欢迎信息显示了一些基本的硬件信息。如下：

![](https://cdn.jsdelivr.net/gh/ahoopia/image/cs/20240126225941.png)

新版本ubuntu已经支持动态的motd. 路径为`/etc/update-motd.d`，里面按照序号有多个文件。用户可以往里面添加脚本实现自定义欢迎信息。

![](https://cdn.jsdelivr.net/gh/ahoopia/image/cs/20240126230159.png)

除此之外，有两个服务也广受欢迎，它们分别是neofetch 和screenfetch。

### neofetch

可以直接通过`sudo apt install neofetch ` 进行安装。

可以将其写入到`/etc/profile.d` 路径，登录成功即可显示。效果如下：

![](https://cdn.jsdelivr.net/gh/ahoopia/image/cs/20240126230821.png)

### screenfetch

用法同上，安装命令为`sudo apt install screenfetch`.

