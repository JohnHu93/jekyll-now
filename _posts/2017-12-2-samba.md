---
layout: post
title: 将Ubuntu中的文件共享给Windows
---

之前一直使用putty中的pscp在Windows和Ubuntu来导传文件。最近发现可以使用samba来将文件直接共享给Windows，这样查看Ubuntu中的文件效率就会高很多。

下面来介绍下方法：
1. 安装samba
	```shell
	sudo apt-get update
	sudo apt-get install samba
	```
1. 为你的samba创建用户和密码：
	```shell
	sudo smbpasswd -a <user_name>
	```
