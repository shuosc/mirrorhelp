#  CRAN镜像帮助 

**CRAN (The Comprehensive R Archive Network)** 镜像源配置文件之一是`.Rprofile` (**linux** 下位于` ~/.Rprofile` )。

在文末添加如下语句:

```bash
options("repos" = c(CRAN="https://mirrors.shuosc.org/CRAN/"))
```

打开 R 即可使用该 `CRAN `镜像源安装 R 软件包。