#  Docker Community Edition镜像使用帮助

> 注意：本镜像只提供Debian/Ubuntu/Fedora/CentOS/RHEL的docker软件包，非dockerhub

###  Debian/Ubuntu用户 

如果你过去安装过**docker**，先删掉：
    sudo apt-get remove docker docker-engine docker.io
首先安装依赖：    
    sudo apt-get install apt-transport-https ca-certificates curl gnupg2 software-properties-common
信任**Docker**的**GPG**公钥：
    curl -fsSL https://mirrors.shuosc.org/docker-ce/linux/debian/gpg | sudo apt-key add -
对于**amd64**架构的计算机，添加软件仓库：
    sudo add-apt-repository \ 
         "deb [arch=amd64] https://mirrors.shuosc.org/docker-ce/linux/debian" \
         $(lsb_release -cs) \
         stable"
如果你是树莓派或其他**ARM**架构计算机，请运行：
    echo "deb [arch=armhf] https://mirrors.shuosc.org/docker-ce/linux/debian \
     $(lsb_release -cs) stable" | \
    sudo tee /etc/apt/sources.list.d/docker.list
最后安装
    sudo apt-get update
    sudo apt-get install docker-ce
###  Fedora/CentOS/RHEL

如果你之前安装过**docker**，请先删掉：

  ```bash
sudo yum remove docker docker-common docker-selinux docker-engine
  ```

安装一些依赖

```bash
sudo yum install -y yum-utils device-mapper-persistent-data lvm2
```

根据你的发行版下载`repo`文件： 
如果你是**centos**：

    wget -O /etc/yum.repos.d/docker-ce.repo https://mirrors.shuosc.org/docker-ce/linux/centos/docker-ce.repo
    sudo sed -i 's+download.docker.com+mirrors.shuosc.org/docker-ce+' /etc/yum.repos.d/docker-ce.repo
如果你是**fedora**：   
    wget -O /etc/yum.repos.d/docker-ce.repo https://mirrors.shuosc.org/docker-ce/linux/fedora/docker-ce.repo
    sudo sed -i 's+download.docker.com+mirrors.shuosc.org/docker-ce+' /etc/yum.repos.d/docker-ce.repo
最后安装：
    sudo yum makecache fast
    sudo yum install docker-ce
