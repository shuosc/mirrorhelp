# Pritunl 镜像使用帮助

**Pritunl**是国外**Pritunl公司**提供的一款企业级的**开源OpenVPN**实现方案，搭建简单、方便。本镜像是直接从**Pritunl官方源**全量同步过来的。

### 使用方法

- Ubuntu

```bash
sudo tee -a /etc/apt/sources.list.d/postgresql.list << EOF
deb https://mirrors.shuosc.org/postgresql/repos/apt/ xenial-pgdg main
EOF
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv 7FCC7D46ACCC4CF8
sudo apt update
sudo apt install postgresql
```
- Centos 7
```bash
sudo yum install https://mirrors.shuosc.org/postgresql/repos/yum/10/redhat/rhel-7-x86_64/pgdg-centos10-10-1.noarch.rpm
sudo yum install postgresql10
```


### 相关链接

- 官网：https://www.postgresql.org