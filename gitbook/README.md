# GitBook 使用教程

## 背景

由于之前都把零散的知识都写在 [Gist](https://gist.github.com) 上，要查找的时候不是很系统化，所以打算挪到 [GitBook](https://www.gitbook.com) 上来统一管理，而且 [GitBook](https://www.gitbook.com) 写完编译后可以生成静态页面发布到博客上，逼格满满的样子。


## GitBook 简介

[GitBook 官网](https://www.gitbook.com)
[GitBook 文档](https://github.com/GitbookIO/gitbook)


## GitBook 准备工作

### 安装 Node.js

GitBook 是一个基于 Node.js 的命令行工具，下载安装 [Node.js](https://nodejs.org/en)，安装完成之后，你可以使用下面的命令来检验是否安装成功。

```
$ node -v
v7.7.1
```


### 安装 GitBook

输入下面的命令来安装 GitBook。

```
$ npm install gitbook-cli -g
```

安装完成之后，你可以使用下面的命令来检验是否安装成功。

```
$ gitbook -V
CLI version: 2.3.2
GitBook version: 3.2.3
```

更多详情请参照 [GitBook 安装文档](https://github.com/GitbookIO/gitbook/blob/master/docs/setup.md) 来安装 GitBook。


### 安装 GitBook 编辑器

去 [GitBook 官网](https://www.gitbook.com/) 下载 GitBook 编辑器；如果是 Mac 用户且安装过 `brew cask` 的话可以使用 `brew cask install gitbook-editor` 命令行来安装 GitBook 编辑器。


## 预览书籍

用 GitBook 编辑器写完之后运行如下命令即可在 http://localhost:4000/ 预览书籍。

```
$ gitbook serve
```

运行该命令后会在书籍的文件夹中生成一个 `_book` 文件夹, 里面的内容即为生成的 html 文件，我们可以使用下面命令来生成网页而不开启服务器。

```
gitbook build
```


## GitBook 配置
