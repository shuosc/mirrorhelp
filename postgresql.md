# Postgresql 镜像使用帮助

**Postgresql**是一款非常流行的关系型数据库。

### 使用方法

- Ubuntu

```bash
sudo tee -a /etc/apt/sources.list.d/postgresql.list << EOF
deb https://mirrors.shu.edu.cn/postgresql/repos/apt/ xenial-pgdg main
EOF
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv 7FCC7D46ACCC4CF8
sudo apt update
sudo apt install postgresql
```

- Centos 7

```bash
sudo yum install https://mirrors.shu.edu.cn/postgresql/repos/yum/10/redhat/rhel-7-x86_64/pgdg-centos10-10-1.noarch.rpm
sudo yum install postgresql10
```


### 相关链接

- 官网：https://www.postgresql.org