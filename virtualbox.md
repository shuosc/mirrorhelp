# Virtualbox 源使用帮助

### 地址

https://mirrors.shuosc.org/virtualbox

### 说明

Virtualbox 是一款开源虚拟机软件，原来是由Sun Microsystems 公司出品，采用Qt编写，后由于Sun被Oracle收购后正式更名为 Oracle VM VirtualBox，并以GPL协议开源。

### 使用说明

#### Windows安装或Mac安装

请在镜像站主页使用快速下载工具选择下载安装即可

#### Linux安装

建议通过包管理器安装

- Debian/Ubuntu 用户

对于 Debian 8 和 Ubuntu 16.04 及以上：
```bash
wget -q https://mirrors.shuosc.org/virtualbox/debian/oracle_vbox_2016.asc -O- | sudo apt-key add -
```
其他版本
```bash
wget -q https://mirrors.shuosc.org/virtualbox/debian/oracle_vbox.asc -O- | sudo apt-key add -
```
再以 `Ubuntu 16.04 LTS` 为例，将文本框中内容写进`/etc/apt/sources.list.d/virtualbox.list`
```bash
deb https://mirrors.tuna.tsinghua.edu.cn/virtualbox/apt/ xenial contrib
```
安装 VirtualBox:
```bash
sudo apt-get update
sudo apt-get install virtualbox-5.2
```

- RHEL/CentOS 用户

新建 `/etc/yum.repos.d/virtualbox.repo`，内容为
```bash
[virtualbox]
name=Virtualbox Repository
baseurl=https://mirrors.shuosc.org/virtualbox/rpm/el$releasever/
gpgcheck=0
enabled=1
```
刷新缓存并安装 `virtualbox` 即可。
```bash
sudo yum makecache
sudo yum install VirtualBox-5.2
```

### 相关链接

- 官方主页：https://www.virtualbox.org/