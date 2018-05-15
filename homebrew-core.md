# Homebrew-core镜像帮助 

### 地址 

- https://mirrors.shu.edu.cn/homebrew-core （仅HTTP/HTTPS访问，不支持git拉取）
- https://mirrors.shu.edu.cn/mgit/homebrew-core (仅git访问)
- ~~https://git.shuosc.org/Homebrew/homwbrew-core （均支持）~~

### 说明 

Homebrew-core镜像

### 使用说明

#### 方式一：使用主站 Nginx 代理git

```bash
# 替换现有上游
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.shu.edu.cn/mgit/homebrew-core
```

#### 方式二：使用 Gitlab 仓库镜像 (已废弃)

```bash
# 替换现有上游
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://git.shuosc.org/Homebrew/brew.git
```

#### 重置为官方上游

```bash
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://github.com/Homebrew/homebrew-core.git
```

### 相关链接 

- 官方主页：https://github.com/Homebrew/homebrew-core