# Pritunl 镜像使用帮助

**Pritunl**是国外**Pritunl公司**提供的一款企业级的**开源OpenVPN**实现方案，搭建简单、方便。本镜像是直接从**Pritunl官方源**全量同步过来的。

### 使用方法

```bash
sudo tee -a /etc/apt/sources.list.d/pritunl.list << EOF
deb https://mirrors.shu.edu.cn/pritunl/stable/apt xenial main
EOF

sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv 7568D9BB55FF9E5287D586017AE645C0CF8E292A

sudo tee -a /etc/apt/sources.list.d/mongodb.list << EOF
deb https://mirrors.shu.edu.cn/mongodb/apt/ubuntu xenial/mongodb-org/3.4 multiverse
EOF

sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv 0C49F3730359A14518585931BC711F9BA15703C6

sudo apt update
echo y |sudo apt install pritunl mongodb-org
sudo systemctl start pritunl mongod
sudo systemctl enable pritunl mongod

# 生成安装秘钥 
sudo pritunl setup-key

# Ubuntu安装客户端
sudo apt-get install pritunl-client-gtk
```
### 相关链接

- 官方主页: https://pritunl.com