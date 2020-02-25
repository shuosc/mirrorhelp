### Zabbix镜像使用帮助

**注意：本镜像只提供Debian/Ubuntu/CentOS/RHEL的zabbix软件包**

### Debian/Ubuntu用户

- 信任zabbix的GPG公钥并新增源文件zabbix.list：

```bash
curl -fsSL https://mirrors.shuosc.cn/zabbix/zabbix-official-repo.key | sudo apt-key add -
echo "deb https://mirrors.shuosc.cn/zabbix/zabbix/3.4/ubuntu/ $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/zabbix.list
```

- 最后安装

```bash
sudo apt-get update
sudo apt-get install zabbix-agent
```
### CentOS/RHEL用户

- 如果你是centos/redhat：

```bash
sudo tee -a /etc/yum.repos.d/zabbix.repo >> EOF
[zabbix]
name=zabbix - $basearch
baseurl=https://mirrors.shuosc.cn/zabbix/zabbix/3.4/rhel/7/$basearch/stable
enabled=1
gpgcheck=1
gpgkey=https://mirrors.shuosc.cn/zabbix/RPM-GPG-KEY-ZABBIX
EOF
```
- 最后安装：

```bash
sudo yum makecache fast
sudo yum install zabbix-agent
```
### 相关链接

- 官方主页: https://www.zabbix.com/