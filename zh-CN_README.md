# Android 口袋开发环境部署教程(用你的安卓手机自由编程)
考虑到外出调试和运维Linux服务器以及用手机学习Linux下的编程，作者(闲得无聊)折腾了一下Android下能否实现vim以及自动补全功能

## 安装过程
- 首先，从应用商店下载安装Termux(仅限Android用户,IOS用户请使用SSH到VPS的方法) 
打开Termux
### 安装Atilo
> 什么是Atilo?<br>
> Atilo 是一个用来帮助你在termux上安装不同的GNU/Linux发行版的程序 

- 输入以下命令 
```bash
echo "deb [trusted=yes arch=all] https://yadominjinta.github.io/files/ termux extras" >> $PREFIX/etc/apt/sources.list
pkg in atilo-cn
```
- 更多关于Atilo安装配置[点击这里](https://github.com/YadominJinta/atilo/blob/master/README.md)

- 在Atilo选择你需要的Linux发行版
```bash
Atilo           2.0
Usage: atilo [命令] [参数]

Atilo 是一个用来帮助你在termux上安装不同的GNU/Linux发行版的程序

命令:
images           列出可用镜像
remove           移除本地的镜像
pull             拉取远的镜像
run              运行镜像
clean            清除缓存
help             帮助
```
- 简单来说，运行以下命令即可
```
atilo pull [你需要的Linux发行版]
atilo run [刚刚获取的Linux镜像]
```
### 安装 VIM & Youcompleteme
> YouCompleteMe，这是一个自动补全工具，对比了一下在一些深度学习第三方库的自动补全速度超过pycharm，例如tensorflow。在其他的Python库的补全速度方面也远远超过vs code

- 由于我日常使用的是Ubuntu20.04LTS，在Ubuntu下VIM和Youcompleteme是很容易通过以下命令安装的 
```bash
apt-get install vim vim-youcompleteme
```
- 这个命令的好处在于无需从源代码编译安装Youcompleteme

- 其他发行版我还没有测试过，不过理论上都可以从源码编译安装Youcompleteme
### 配置VIM和Youcompleteme
配置文件已经传到我的Github
My vimrc is [Here](https://github.com/zhzhzhy/My_vimrc)
