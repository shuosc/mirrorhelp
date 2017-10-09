# Mongodb源使用帮助

### 地址

https://mirrors.shuosc.org/mongodb

### 说明

**Mongodb**是一款流行的开源非关系型数据库软件

### 使用说明

- Debian/Ubuntu等使用

  ```bash
sudo tee -a /etc/apt/sources.list.d/mongodb.list << EOF
deb https://mirrors.shuosc.org/mongodb/apt/ubuntu xenial/mongodb-org/3.4 multiverse
EOF

sudo apt-key adv --keyserver hkp://pgp.mit.edu --recv 0C49F3730359A14518585931BC711F9BA15703C6

sudo apt update
  ```

- Centos/Fedora等使用

   ```bash
sudo tee -a /etc/yum.repos.d/mongodb.repo << EOF
[mongodb]
name=Mongodb Stable Repository
baseurl=https://mirrors.shuosc.org/mongodb/yum/redhat/7/mongodb-org/3.4/x86_64/
gpgcheck=1
enabled=1
EOF

gpg --keyserver hkp://pgp.mit.edu --recv-keys 0C49F3730359A14518585931BC711F9BA15703C6

sudo yum makecache
   ```

### 相关链接

- 官方主页：https://mongodb.org