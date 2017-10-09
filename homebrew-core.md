# Homebrew-core镜像帮助 

### 地址 

https://git.shuosc.cn/Homebrew/homebrew-core

### 说明 

Homebrew-core镜像

### 使用说明

* 替换现有上游

```bash
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://git.shuosc.cn/Homebrew/homebrew-core.git
```

* 重置为官方上游 

```bash
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://github.com/Homebrew/homebrew-core.git
```

### 相关链接 

- 官方主页：https://github.com/Homebrew/homebrew-core