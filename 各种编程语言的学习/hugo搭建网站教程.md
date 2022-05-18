# 手把手教你用Hugo制作个人网站

## 前期准备
### homebrew安装
#### homebrew介绍
homebrew是Mac的包管理器，能够免去安装软件过程中的注册账号、寻找版本、下载、解压、安装等步骤，直接使用简单的命令行即可安装软件安装包。
#### homebrew的安装
按下`command+space`调出spotlight，在输入框中输入`终端`或`terminal`打开终端，在终端中输入如下命令行，即可下载安装homebrew。
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
看到`==> Installation successful!`就说明安装成功了。

若碰到homebrew安装相关问题可点击[此处](https://www.cnblogs.com/xibushijie/p/13335988.html)查看部分相应的解决办法。
### git安装及配置
#### git安装
在安装好homebrew的基础上，就可以使用指令来安装git了。在终端中输入如下命令：
``` 
brew install git 
```
当在终端窗口中输入`git`后，窗口中出现有关git的用法说明，即说明安装成功。
除以上方法外，你还可以参考[官方安装指导](https://git-scm.com/download/mac)使用其他方法进行安装。
#### git配置
1. 用户信息配置
安装完成后，输入如下命令与github账号绑定（将双引号中的账号信息对应更改为自己的github账号信息）：
```
git config --global user.name "example name"           
git config --global user.email "example@example.com  
```
2. SSH key配置
输入如下代码创建ssh key:
```
ssh-keygen -t rsa -C "example@example.com"
```
按照终端窗口的提示敲击`enter`键，直至其恢复至等待命令状态，然后输入如下命令查询创建的ssh public key：
```
cat id_rsa.pub
```
记录下终端窗口出现的密钥。

3. 远端仓库添加密钥



### hugo安装
同上git安装，在终端中输入：
```
brew install hugo
```
## 网站搭建及配置

### 本地网站的快速搭建
在想创建的文件目录下打开终端，输入：
```
hugo new site Filename 
```
`Filename`可以自己任意命名，运行完该命令后，会在终端运行的目录下新建一个名为`Filename`的文件夹，文件夹内包含网站的所有内容文件，且作为网站根目录。

### 主题的使用
进入[hugo主题页面](https://themes.gohugo.io)选择自己喜爱的主题,本文以[stack主题](https://themes.gohugo.io/themes/hugo-theme-stack/)为例


### 主题的配置
#### 配置文件变量说明
#### 主题其他部分文件说明
### 在线网站搭建
#### 在线网站文件生成
#### 建立github仓库并与本地同步


