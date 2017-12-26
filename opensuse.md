# openSUSE 源使用帮助

### 地址

https://mirrors.shu.edu.cn/opensuse/

### 说明

openSUSE 软件源

### 收录架构

- i586
- x86_64

### 使用说明

手动配置软件源

> 以下配置方法适用于从未自行配置软件源的用户，其他用户请根据具体情况自行配置 ，以下仅供参考。

禁用原有软件源

```bash
sudo zypper mr -da 
```

添加上大镜像源，以 **openSUSE Leap 42.2** 为例；

```bash
sudo zypper ar -fc https://mirrors.shu.edu.cn/opensuse/distribution/leap/42.2/repo/oss USTC:42.2:OSS
sudo zypper ar -fc https://mirrors.shu.edu.cn//opensuse/distribution/leap/42.2/repo/non-oss USTC:42.2:NON-OSS
sudo zypper ar -fc https://mirrors.shu.edu.cn//opensuse/update/leap/42.2/oss USTC:42.2:UPDATE-OSS
sudo zypper ar -fc https://mirrors.shu.edu.cn//opensuse/update/leap/42.2/non-oss USTC:42.2:UPDATE-NON-OSS
```

命令中最后一个参数为每一个源指定了一个 **alias （别称**），可以根据个人喜好更改。

手动刷新软件源

```bash
sudo zypper ref
```

### 相关链接

  * 官方主页: https://www.opensuse.org/
  * 邮件列表: https://en.opensuse.org/Communicate/Mailinglists
  * 论坛: https://forums.opensuse.org/
  * 中文论坛: https://forum.suse.org.cn/
  * Wiki: https://en.opensuse.org/
  * 中文 Wiki: https://zh.opensuse.org/
  * 文档: https://en.opensuse.org/Documentation
  * openSUSE Guide: https://lug.ustc.edu.cn/sites/opensuse-guide/