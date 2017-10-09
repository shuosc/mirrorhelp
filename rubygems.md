# Rubygems源使用帮助

### 地址

https://mirrors.shuosc.org/rubygems

### 说明

Rubygems仓库镜像

### 使用说明 

- 修改Rubygems镜像源 

```bash
gem sources  #列出默认源
gem sources --remove https://rubygems.org/  #移除默认源
gem sources -a https://mirrors.shuosc.org/rubygems/  #添加上大源
```

- 针对使用 Gemfile 和 Bundle 的项目

  ```bash
bundle config mirror.https://rubygems.org https://mirrors.shuosc.org/rubygems/
  ```

### 相关链接

- 官方主页：https://rubygems.org/