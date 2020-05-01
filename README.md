# git克隆远程仓库的指定分支
普通克隆方式：

git clone <远程仓库地址>
复制代码
这种克隆方式默认是克隆master主分支， 而且通过命令 git branch --list 能看到克隆后在本地也只有这一个分支， 如果再通过新建分支再拉取指定分支，甚至可能还需要解决冲突，太繁琐。

那么，如何快速有效的直接克隆远程指定分支？

只需要一条命令：

git clone -b <指定分支名> <远程仓库地址>
复制代码
会自动在克隆该分支在本地，同样克隆后本地只有这一个分支。



# 如何新建分支
1、新建Repository名为xxx
   新建gh-pages分支


2、克隆到本地

>git clone https://github.com/user/xxx.git

3、创建并跟踪gh-pages分支

>git checkout -b gh-pages origin/gh-pages
     

4、同步到远程服务器

>git status

>git add .

>git commit -m "updated"

>git push origin gh-pages


5、通过[URL](https://user.github.io/xxx/)访问

# 重装电脑后，或者在其它电脑上想修改博客

1、
>安装git

>安装Nodejs和npm

>添加ssh-keys

2、克隆到本地

>git clone https://github.com/user/xxx.git

3、创建并跟踪gh-pages分支

>git checkout -b gh-pages origin/gh-pages
     

4、同步到远程服务器

>git status

>git add .

>git commit -m "updated"

>git push origin gh-pages
