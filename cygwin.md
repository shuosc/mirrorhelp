# Cygwin 源使用帮助

### 地址

https://mirrors.shuosc.cn/cygwin

### 说明

**Cygwin**是一个在windows平台上运行的类UNIX模拟环境，是cygnus solutions公司开发的自由软件（该公司开发的著名工具还有eCos，不过现已被Redhat收购）。

### 使用方法

选择`Install from Internet`, 在`User URL`处输入以下地址，注意，Cygwin貌似不支持使用`https`。(但由于setup.exe是以https链接分发，而镜像文件中又有.sig签名文件，所以可以认为http的镜像是安全的)
```bash
http://mirrors.shuosc.cn/cygwin/
```
点击`Add`按钮，然后选中`http://mirrors.shuosc.cn`，点击`下一步`进行安装。

注意，该列表为可多选列表，注意把上面不需要的镜像关掉。

### 相关链接

- 官方主页：https://cygwin.com
- 64位安装包：https://cygwin.com/setup-x86_64.exe
- 32位安装包：https://cygwin.com/setup-x86.exe