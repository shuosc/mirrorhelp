# Repoforge镜像使用帮助

### 地址

https://mirrors.shu.edu.cn/repoforge

### 说明

原Rpmforge镜像，现改名为Repoforge，是 RHEL 系统下的软件仓库，拥有 10000 多个软件包，被认为是最安全、最稳定的一个软件仓库。

### 使用说明

- 添加 **Repoforge** 仓库 

运行`cat /etc/redhat-release`获取 EL 版本号（如 EL6, EL7 等）
向系统中添加 **Repoforge** 的 **GPG 公钥**：

```bash
rpm --import https://mirrors.shu.edu.cn/repoforge/RPM-GPG-KEY.dag.txt
```

运行下列命令：

```bash
sudo cat > /etc/yum.repos.d/rpmforge.repo << EOF
[rpmforge]
name = RHEL $releasever - RPMforge.net - dag
baseurl = https://mirrors.shu.edu.cn/repoforge/redhat/el7/en/$basearch/rpmforge
mirrorlist = http://mirrorlist.repoforge.org/el7/mirrors-rpmforge
enabled = 1
protect = 0
gpgkey = file:///etc/pki/rpm-gpg/RPM-GPG-KEY-rpmforge-dag
gpgcheck = 1

[rpmforge-extras]
name = RHEL $releasever - RPMforge.net - extras
baseurl = https://mirrors.shu.edu.cn/repoforge/redhat/el7/en/$basearch/extras
mirrorlist = http://mirrorlist.repoforge.org/el7/mirrors-rpmforge-extras
enabled = 0
protect = 0
gpgkey = file:///etc/pki/rpm-gpg/RPM-GPG-KEY-rpmforge-dag
gpgcheck = 1

[rpmforge-testing]
name = RHEL $releasever - RPMforge.net - testing
baseurl = https://mirrors.shu.edu.cn/repoforge/redhat/el7/en/$basearch/testing
mirrorlist = http://mirrorlist.repoforge.org/el7/mirrors-rpmforge-testing
enabled = 0  
protect = 0
gpgkey = file:///etc/pki/rpm-gpg/RPM-GPG-KEY-rpmforge-dag
gpgcheck = 1

EOF
```

- 更新软件包缓存 

```bash
sudo yum makecache
```

### 相关链接

- 官方主页：https://repoforge.rog