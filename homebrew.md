#  Homebrew镜像帮助

###  地址 

- https://mirrors.shu.edu.cn/brew （仅HTTP/HTTPS访问，不支持git拉取）
- https://mirrors.shu.edu.cn/mgit/brew (仅git访问)
- ~~https://git.shuosc.org/Homebrew/brew （均支持）~~

###  说明

Homebrew镜像

### 使用说明 

目前本镜像站提供两种方式替换上游。

#### 方式一：使用主站 Nginx 代理git

```bash
# 替换现有上游
cd "$(brew --repo)"
git remote set-url origin https://mirrors.shu.edu.cn/mgit/brew
```

#### 方式二：使用 Gitlab 仓库镜像 (已废弃)

```bash
# 替换现有上游
cd "$(brew --repo)"
git remote set-url origin https://git.shuosc.org/Homebrew/brew.git
```

#### 重置为官方上游

```bash
# 重置为官方上游 
cd "$(brew --repo)"
git remote set-url origin https://github.com/Homebrew/brew.git
```

### 相关链接 

- 官方主页：https://github.com/Homebrew/brew