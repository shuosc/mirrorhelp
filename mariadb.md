# MariaDB 源使用帮助

### 地址

https://mirrors.shuosc.org/mariadb/

### 收录架构

官方支持的所有架构

### 收录版本

官方支持的所有版本

### 使用说明

- Fedora, CentOS, Red Hat

使用[MariaDB Repository Configuration Tool](https://downloads.mariadb.org/mariadb/repositories)生成一份配置，保存为 ``/etc/yum.repos.d/mariadb.repo``

然后执行以下命令替换源地址：

```bash
sudo sed -i 's#yum.mariadb.org#mirrors.shuosc.org/mariadb/yum#' /etc/yum.repos.d/mariadb
```

> 建议使用 HTTPS

```bash
sudo sed -i 's#http://mirrors.shuosc.org#https://mirrors.shuosc.org#g' /etc/yum.repos.d/mariadb
```

- Mint, Ubuntu, Debian

1. 使用[MariaDB Repository Configuration Tool](https://downloads.mariadb.org/mariadb/repositories)生成要执行的命令（Mirror 选择 Babylon Network - NL）
2. 将 ``add-apt-repository`` 命令中的http://nl.mirror.babylon.network替换为 https://mirrors.shuosc.org
3. 执行命令

### 相关链接 

  * MariaDB 官网: https://mariadb.org/
  * MariaDB Repository Configuration Tool: https://downloads.mariadb.org/mariadb/repositories