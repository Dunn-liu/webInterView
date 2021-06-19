# webInterview

#### 介绍
面试题收集, 分享

#### 软件架构
gitbook

#### 说明
改文档基于gitbook 使用前安装gitbook环境

#### gitbook安装教程

GitBook的安装非常简单。您的系统只需满足这两个要求：

- NodeJS（推荐使用v4.0.0及以上版本,v10.0.0以下版本）
- Windows，Linux或Mac OS X

### 安装 Node.js

首先我们需要做的是安装 Node.js,这里不再赘述,推荐使用 nvm 进行node版本管理(自行官网下载安装) 安装前最好先卸载本机已安装node
常用nvm命令
```bash
nvm list // 查看本机已安装node版本
nvm list available  // 查看远程可安装使用node版本
nvm install version  // 安装指定版本node
nvm uninstall version  // 卸载指定版本node
nvm use version // 切换使用指定版本node
```

### Node.js 镜像配置

`Node.js` 安装完成后，我们就可以开始安装 gitbook 了。但是在安装之前，最好先配置一下`Node.js` 源的下载镜像地址。

因为默认的镜像地址是在国外，国内访问速度极慢，因此我们需要设置国内的镜像地址。

国内的我推荐大家使用阿里巴巴的镜像地址 `http://registry.npm.taobao.org` 。

执行下面的命令，进行配置：

`npm config set registry http://registry.npm.taobao.org`


### 安装 gitbook

执行命令：
`npm install gitbook-cli -g`

`gitbook-cli` 是安装和管理GitBook版本库的程序。它会自动安装GitBook所需的模块来创建一本书。

安装完成后，可以执行 `gitbook --version` 查看安装的版本信息。

```x86asm
C:\Users\admin>gitbook --version
CLI version: 2.3.2
GitBook version: 3.2.3
```

### 安装其他版本

使用`gitbook ls-remote`列出可用于安装的远程版本。

```x86asm
C:\Users\admin>gitbook ls-remote
Available GitBook Versions:

     4.0.0-alpha.6, 4.0.0-alpha.5, 4.0.0-alpha.4, 4.0.0-alpha.3, 4.0.0-alpha.2, 4.0.0-alpha.1, 3.2.3....

Tags:

     latest : 2.6.9
     pre : 4.0.0-alpha.6
```

使用 `gitbook fetch` 可以来指定需要获取的版本。

`gitbook fetch 4.0.0-alpha.6`


#### 安装教程

1.  git clone url
2.  cd docs
3.  gitbook install 安装插件
4.  开始修改文件

#### 使用说明

1.  /docs/SUMMARY.md为侧边目录文件
2.  /docs/information.md 前言介绍
3.  /docs/book.json 配置文件,可添加插件
4.  /docs/assets 放置静态资源文件

