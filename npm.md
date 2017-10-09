# NPM镜像使用帮助


**SHUOSC镜像站**的 `npm` 镜像是 基于`cnpm`搭建的https://registry.npmjs.org/ 的反向代理。

### 使用说明

编辑`~/.npmrc`，添加

```bash
registry=https://registry.npm.shuosc.org/
```

若不想将本源设置为默认源，只想使用本源安装某个软件包，可在安装包时采用以下用法：

```bash
npm --registry https://registry.npm.shuosc.org install <packagename>
```

**SHUOSC镜像站**可以使用`cnpm'`命令来代替`npm`命令，更加方便，详情请转至[npm镜像站](https://npm.shuosc.org)查看。

### 注意事项

不支持 **publish**，若出现错误，请将 `~/.npmrc` 中的用户名密码部分注释掉，并删除缓存`rm -rf ~/.npm` 重试。

### 相关链接

- 官方主页: https://www.npmjs.org/ 
- cnpm主页：https://cnpmjs.org/ 
- Github主页：https://github.com/cnpm/cnpm