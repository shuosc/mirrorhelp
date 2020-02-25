#  CRAN镜像帮助 

### 地址

https://mirrors.shuosc.cn/CRAN/

### 使用说明

#### 方式一：自定义配置文件

**CRAN (The Comprehensive R Archive Network)** 镜像源配置文件之一是`.Rprofile` (**linux** 下位于` ~/.Rprofile` )。

在文末添加如下语句:

```bash
options("repos" = c(CRAN="https://mirrors.shuosc.cn/CRAN/"))
```

打开 R 即可使用该 `CRAN `镜像源安装 R 软件包。

#### 方式二：界面选择

步骤一：进入全局选项设置

![vgy.me](https://vgy.me/yAKVYC.png)

步骤二：选择`China (Shanghai 2) [https] - Shanghai University`

![vgy.me](https://vgy.me/lWMmbH.png)

步骤三：点击`OK`按钮，可以畅快地安装 R 软件包了。