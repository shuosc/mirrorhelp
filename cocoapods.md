# CocoaPods 镜像帮助

###  地址

- https://mirrors.shu.edu.cn/CocoaPods （仅HTTP/HTTPS访问，不支持git拉取）
- https://mirrors.shu.edu.cn/git/specs (仅git访问)
- https://git.shuosc.org/CocoaPods/Specs （均支持）


### 说明 

CocoaPods/Specs 镜像

### 使用说明

#### 方式一：使用主站 Nginx 代理git

```bash
# 替换现有上游
cd ~/.cocoapods/repos
pod repo remove master
git clone https://mirrors.shu.edu.cn/git/specs master

# 最后进入自己的工程，在自己工程的podFile第一行加上
source 'https://mirrors.shu.edu.cn/git/specs'
```

#### 方式二：使用 Gitlab 仓库镜像

```bash
# 替换现有上游
cd ~/.cocoapods/repos
pod repo remove master
git clone https://git.shuosc.org/CocoaPods/Specs master

# 最后进入自己的工程，在自己工程的podFile第一行加上
sources 'https://git.shuosc.org/CocoaPods/Specs'
```

#### 重置为官方上游

```bash
cd ~/.cocoapods/repos
pod repo remove master
git clone https://github.com/CocoaPods/Specs master

# 最后进入自己的工程，在自己工程的podFile第一行加上
sources 'https://github.com/CocoaPods/Specs'
```

### 相关链接

- 官方主页：https://github.com/CocoaPods/Specs