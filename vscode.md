# Vscode源使用帮助

### 地址

https://mirrors.shuosc.cn/vscode

### 说明

由Microsoft公司开发的IDE神器----**VSCODE**，自发布以来深受广大开发者喜爱。目前社区比较活跃，各式各样的插件源源不断，非常适合喜欢简洁的开发者。

### 使用说明 

- Debian 和 Ubuntu 一类发行版

```bash
curl https://mirrors.shuosc.cn/vscode/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
sudo sh -c 'echo "deb [arch=amd64] https://mirrors.shuosc.cn/vscode/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
sudo apt-get update
sudo apt-get install code # or code-insiders
```

- RHEL, Fedora 和 CentOS 一类发行版


```bash
sudo rpm --import https://mirrors.shuosc.cn/vscode/keys/microsoft.asc
sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://mirrors.shuosc.cn/vscode/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://mirrors.shuosc.cn/vscode/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'

# 使用dnf管理工具的执行下面命令安装vscode
dnf check-update
sudo dnf install code

# 使用yum管理工具的执行下面命令安装vscode
yum check-update
sudo yum install code
```

- openSUSE 和 SLE 一类发行版

```bash
sudo rpm --import https://mirrors.shuosc.cn/vscode/keys/microsoft.asc
sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://mirrors.shuosc.cn/vscode/yumrepos/vscode\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://mirrors.shuosc.cn/vscode/keys/microsoft.asc" > /etc/zypp/repos.d/vscode.repo'
sudo zypper refresh
sudo zypper install code
```


### 相关链接

- 官方主页：https://code.visualstudio.com/
- Linux安装指南：https://code.visualstudio.com/docs/setup/linux