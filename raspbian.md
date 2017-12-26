# Raspbian 源使用帮助

### 地址

https://mirrors.shu.edu.cn/raspbian

### 说明

Raspbian 是专门用于 ARM 卡片式计算机 Raspberry Pi® “树莓派”的操作系统。

### 收录架构

- armhf：wheezy、jessie

### 使用说明

使用管理员权限（sudo），编辑 `/etc/apt/sources.list` 文件。参考命令行为：
```bash
pi@raspberrypi ~ $ sudo nano /etc/apt/sources.list
```
删除原文件所有内容，用以下内容取代：

以`jessie版本`为例：
```bash
deb https://mirrors.shu.edu.cn/raspbian/raspbian/ jessie main non-free contrib
deb-src https://mirrors.shu.edu.cn/raspbian/raspbian/ jessie main non-free contrib
```

> 注意：网址末尾的`raspbian`重复两次是必须的。因为Raspbian的仓库中除了APT软件源还包含其他代码。APT软件源不在仓库的根目录，而在raspbian/子目录下。

编辑镜像站后，请使用  `sudo apt-get update` 命令，更新软件源列表，同时检查您的编辑是否正确。

### 声明

Raspbian是由独立开发者维护的，与树莓派硬件的开发与维护者The Raspberry Pi Foundation“树莓派基金会”并无直接联系。

### 相关链接

- 官方主页：http://www.raspbian.org/
- 官方文档：http://www.raspbian.org/RaspbianDocumentation
- Bug Tracker：http://www.raspbian.org/RaspbianBugs
- 镜像列表：http://www.raspbian.org/RaspbianMirrors