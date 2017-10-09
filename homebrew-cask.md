# Homebrew-cask镜像帮助

###  地址

https://git.shuosc.cn/caskroom/homebrew-cask

### 说明 

Homebrew-cask镜像

### 使用说明

* 替换现有上游 

```bash
cd "$(brew --repo)"/Library/Taps/caskroom/homebrew-cask
git remote set-url origin https://git.shuosc.org/caskroom/homebrew-cask.git
```

* 重置为官方上游 

```bash
cd "$(brew --repo)"/Library/Taps/caskroom/homebrew-cask
git remote set-url origin https://github.com/caskroom/homebrew-cask
```

### 相关链接

- 官方主页：https://github.com/caskroom/homebrew-cask