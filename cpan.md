# CPAN 源使用帮助

### 地址

https://mirrors.shu.edu.cn/CPAN

### 说明

**CPAN**是`Perl程序库`，包含了很多用Perl写成的软件和其他文件，适用于不同操作系统。

### 使用说明

如果以前从未使用过CPAN，请在命令行下运行`cpan`
```bash
Would you like to configure as much as possible automatically? [yes]
```
此处输入`no`
```bash
Would you like to pick from the CPAN mirror list? [yes] 
```
此处直接回车，在列表中选择`Asia`、`China`、`http://mirrors.shu.edu.cn/CPAN/`

如果你已经使用过CPAN了，那么直接修改`~/.cpan/CPAN/MyConfig.pm`中的`urllist`的值为
```bash
'urllist' => [q[http://mirrors.shu.edu.cn/CPAN/]],
```


### 相关链接

- 官方主页：http://www.cpan.org
- 镜像列表：http://www.cpan.org/SITES.html
- FAG：http://www.cpan.org/misc/cpan-faq.html