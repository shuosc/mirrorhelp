#  Homebrew镜像帮助

###  地址 

https://git.shuosc.cn/Homebrew/brew

###  说明

Homebrew镜像

### 使用说明 

```bash
# 替换现有上游
cd "$(brew --repo)"
git remote set-url origin https://git.shuosc.org/Homebrew/brew.git
# 重置为官方上游 
cd "$(brew --repo)"
git remote set-url origin https://github.com/Homebrew/brew.git
```

### 相关链接 

- 官方主页：https://github.com/Homebrew/brew