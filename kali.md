# Kali Linux 源使用帮助

### 地址

https://mirrors.shu.edu.cn/kali/

### 说明

Kali Linux 软件源

### 支持的系统架构

- amd64
- arme
- armhf
- i386

### 使用说明

编辑 `/etc/apt/sources.list` 文件, 在文件最前面添加以下条目：

 ```bash
deb https://mirrors.shu.edu.cn/kali kali-rolling main non-free contrib
deb-src https://mirrors.shu.edu.cn/kali kali-rolling main non-free contrib
 ```

### 相关链接

  * **Kali Linux** 主页: https://www.kali.org/