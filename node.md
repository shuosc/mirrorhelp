# Node 源使用帮助

### 地址

https://mirrors.shuosc.org/node

### 说明

**Node.js**是一个Javascript运行环境(runtime)，发布于2009年5月，由Ryan Dahl开发，实质是对Chrome V8引擎进行了封装。

### 使用说明

#### Windows安装

在镜像站主页的快捷下载工具中选择下载安装包安装即可。

#### Mac安装

- 方法一：同Windows安装
- 方法二：切换到本站提供的`homebrew-bottles`源，再使用`brew install node`即可

#### Linux安装

- 在镜像站主页的快捷下载工具中选择下载`tar.gz`格式压缩包
- 使用`tar zxf *.tar.gz`（`*`为压缩包名）命令解压缩并移动到一个有权限的目录，比如`/home/{user}/nodejs`
- 在`.bashrc`中添加`PATH=/home/{user}/nodejs/bin:$PATH`，并且使用`source .bashrc`生效配置
- `node -v`测试是否安装成功

> 由于目前镜像站的硬盘容量不足，原CNPM镜像站暂停服务，等到空间充足时再行恢复。在此期间，建议转至 https://npm.taobao.org 提供的NPM加速服务


### 相关链接

- 官方主页：https://nodejs.org
- 官方文档：https://nodejs.org/dist/latest-v9.x/docs/api/
- npm主站：https://www.npmjs.com
- 淘宝NPM镜像：https://npm.taobao.org