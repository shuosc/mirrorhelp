# Docker Hub 加速访问镜像使用帮助


### Linux

```bash
curl -sSL https://mirrors.shu.edu.cn/data/set_mirror.sh | sh -s https://docker.mirrors.shu.edu.cn
或
curl -sSL https://mirrors.shu.edu.cn/data/set_mirror.sh | sh -s https://docker.mirrors6.shu.edu.cn
```
该脚本可以将 `--registry-mirror` 加入到你的 `Docker` 配置文件 `/etc/docker/daemon.json` 中。适用于 `Ubuntu14.04`、`Debian`、`CentOS6` 、`CentOS7`、`Fedora`、`Arch Linux`、`openSUSE Leap 42.1`，其他版本可能有细微不同。

### macOS
Docker For Mac

右键点击桌面顶栏的 `docker` 图标，选择 `Preferences` ，在 `Daemon` 标签（`Docker 17.03` 之前版本为 `Advanced` 标签）下的 `Registry mirrors` 列表中加入下面的镜像地址:

```
https://docker.mirrors.shu.edu.cn
或
https://docker.mirrors6.shu.edu.cn
```

点击 `Apply & Restart` 按钮使设置生效。

### Windows

Docker For Windows

在桌面右下角状态栏中右键 `docker` 图标，修改在 `Docker Daemon` 标签页中的 `json` ，把下面的地址:

```bash
https://docker.mirrors.shu.edu.cn
或
https://docker.mirrors6.shu.edu.cn
```

加到 `registry-mirrors` 的数组里。点击 `Apply` 。


### 相关链接 

  * 官方主页: https://hub.docker.com/