# Msys2 源使用帮助

### 地址

https://mirrors.shuosc.cn/msys2

### 说明

### 收录架构

- MINGW: i686，x86_64
- MSYS: i686, x86_64

### 使用说明

请访问该镜像目录下的 `distrib/` 目录（`x86_64` 、`i686`），找到名为 `msys2-<架构>-<日期>.exe` 的文件（如 `msys2-x86_64-20141113.exe`），下载安装即可。

#### pacman 的配置

编辑 `/etc/pacman.d/mirrorlist.mingw32` ，在文件开头添加：
```bash
Server = https://mirrors.shuosc.cn/msys2/mingw/i686
```
编辑 `/etc/pacman.d/mirrorlist.mingw64` ，在文件开头添加：
```bash
Server = https://mirrors.shuosc.cn/msys2/mingw/x86_64
```
编辑 `/etc/pacman.d/mirrorlist.msys` ，在文件开头添加：
```bash
Server = https://mirrors.shuosc.cn/msys2/msys/$arch
```
然后执行 `pacman -Sy` 刷新软件包数据即可。

### 相关链接

- 官方主页：http://www.msys2.org/
- Github主页：https://github.com/msys2