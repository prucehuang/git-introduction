## 提前要求
* NodeJS (要求是10.X版本，更高版本会报错，TypeError: cb.apply is not a function)
* Windows, Linux, Unix, or Mac OS X

## 安装
```
# 安装node
$ brew install node@10
$ echo 'export PATH="/usr/local/opt/node@10/bin:$PATH"' >> ~/.zshrc
$ source ~/.zshrc

# 安装管理工具cli
$ npm install gitbook-cli -g

# 查看并安装最新版本的GitBook
$ gitbook -V
```
`gitbook-cli` 是GitBook的管理工具，能自动下载安装GitBook，并选择不同的版本

## 创建一本书
```
$ gitbook init
# 或者初始化一本书到指定目录
$ gitbook init ./directory
```

## 在本地搭建一个服务器，预览
```
$ gitbook serve
# 本地查看网址
http://localhost:4000/
```

## 其他命令
```
# 安装插件
$ gitbook install
```

```
# 编译生成GitBook Web页面，方便部署到其他地方
$ gitbook build
```

```
# 生成PDF文档（先要安装Calibre软件）
$ gitbook pdf
```
```
# 安装最新测试版本
$ gitbook fetch beta
# 查看远程和本地版本情况
$ gitbook ls-remote
# 打印日志信息
$ gitbook build ./ --log=debug --debug
```

