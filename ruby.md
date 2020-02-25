# Ruby源使用帮助

### 地址

https://mirrors.shuosc.cn/ruby/

### 说明

Ruby源码镜像

### 使用说明 

建议使用`rvm`镜像管理，下面以`Ubuntu 16.04`为例安装。
- 安装`rvm`并配置源 

```bash
gpg --keyserver hkp://pgp.mit.edu --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
curl -sSL https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm

# .zshrc版本
tee -a ~/.zshrc << EOF
[[ -s "$HOME/.rvm/scripts/rvm" ]] && source "$HOME/.rvm/scripts/rvm" 
EOF

# .bashrc版本
tee -a ~/.bashrc << EOF
[[ -s "$HOME/.rvm/scripts/rvm" ]] && source "$HOME/.rvm/scripts/rvm" 
EOF

echo "ruby_url=https://mirrors.shuosc.cn/ruby/ruby" > ~/.rvm/user/db

rvm list known #查看ruby源中支持的版本
```

- 从源码安装**ruby**

```bash
rvm install ruby --disable-binary
ruby -v
```

### 相关链接

- 官方主页：http://www.ruby-lang.org/
- 源码下载地址：http://cache.ruby-lang.org/
- ruby中国：https://ruby-china.org/