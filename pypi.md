# PyPI 镜像使用帮助

> 如何使用上海大学开源镜像站 加速 pip？

编辑 `~/.pip/pip.conf` 文件（如果没有则创建之），将 `index-url `开头的一行修改为下面一行：

```bash
[global]
index-url = https://pypi.shuosc.org/simple

[list]
format = columns
```



### 同步方式

使用`bandersnatch`，每隔6小时从 **pypi.python.org** 官方同步。

### 相关链接 

- PyPI Official Mirrors: https://pypi.python.org/mirrors
- PEP-381 Mirroring Protocol: http://www.python.org/dev/peps/pep-0381/
- bandersnatch: https://pypi.python.org/pypi/bandersnatch