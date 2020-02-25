#  saltstack镜像使用帮助

## Ubuntu系统

```bash
wget -O - https://mirrors.shuosc.cn/saltstack/apt/ubuntu/16.04/amd64/latest/SALTSTACK-GPG-KEY.pub | sudo apt-key add -
sudo tee -a /etc/apt/sources.list.d/saltstack.list << EOF
    deb http://mirrors.shuosc.cn/saltstack/apt/ubuntu/16.04/amd64/latest xenial main
EOF

sudo apt update
sudo apt install salt-master salt-minion salt-ssh salt-cloud salt-api salt-syndic
```

## Debian系统

```bash
wget -O - https://mirrors.shuosc.cn/saltstack/apt/debian/9/amd64/latest/SALTSTACK-GPG-KEY.pub | sudo apt-key add -
sudo tee -a /etc/apt/sources.list.d/saltstack.list << EOF
    deb http://mirrors.shuosc.cn/saltstack/apt/debian/9/amd64/latest stretch main
EOF

sudo apt update
sudo apt install salt-master salt-minion salt-ssh salt-cloud salt-api salt-syndic
```


## Red Hat/Centos系统

```bash
sudo yum install https://mirrors.shuosc.cn/saltstack/yum/redhat/salt-repo-latest-2.el7.noarch.rpm 
sudo yum clean expire-cache

sudo yum install salt-master salt-minion salt-ssh salt-cloud salt-api salt-syndic
```

## Windows系统

下载安装包：
- [64位安装包](https://mirrors.shuosc.cn/saltstack/windows/Salt-Minion-2017.7.2-Py2-AMD64-Setup.exe) [MD5值](https://mirrors.shuosc.cn/saltstack/windows/Salt-Minion-2017.7.2-Py2-AMD64-Setup.exe.md5)
- [32位安装包](https://mirrors.shuosc.cn/saltstack/windows/Salt-Minion-2017.7.2-Py2-x86-Setup.exe) [MD5值](https://mirrors.shuosc.cn/saltstack/windows/Salt-Minion-2017.7.2-Py2-x86-Setup.exe.md5)

## macOS系统

下载安装包： [64位安装包](https://mirrors.shuosc.cn/saltstack/osx/salt-2017.7.2-py2-x86_64.pkg) [MD5值](https://mirrors.shuosc.cn/saltstack/osx/salt-2017.7.2-py2-x86_64.pkg.md5)

安装完后使用以下命令配置：

```bash
# 配置服务
sudo salt-config -i yourminionname -m yoursaltmaster

# 关闭或启动salt服务
sudo launchctl stop com.saltstack.salt.minion
sudo launchctl start com.saltstack.salt.minion
```

## 其他平台

请根据 https://mirrors.shuosc.cn/saltstack/ 的帮助文档，将域名从`repo.saltstack.com`更换成`mirrors.shuosc.cn`即可。