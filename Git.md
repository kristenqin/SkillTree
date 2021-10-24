Git vs SVN

![image](https://www.runoob.com/wp-content/uploads/2015/02/0D32F290-80B0-4EA4-9836-CA58E22569B3.jpg)

Centos安装

命令行安装

```
$ yum install curl-devel expat-devel gettext-devel \
  openssl-devel zlib-devel

$ yum -y install git-core

$ git --version
git version 1.7.1
```
源码安装

```
########## Centos/RedHat ##########
$ yum install curl-devel expat-devel gettext-devel \
  openssl-devel zlib-devel
```
解压

```
$ tar -zxf git-1.7.2.2.tar.gz
$ cd git-1.7.2.2
$ make prefix=/usr/local all
$ sudo make prefix=/usr/local install
```
工作流程

![image](https://www.runoob.com/wp-content/uploads/2015/02/git-process.png)

Git 工作区、暂存区和版本库

![image](https://www.runoob.com/wp-content/uploads/2015/02/1352126739_7909.jpg)

当对工作区修改（或新增）的文件执行 git add 命令时，暂存区的目录树被更新，同时工作区修改（或新增）的文件内容被写入到对象库中的一个新的对象中，而该对象的ID被记录在暂存区的文件索引中。

注： 在 Linux 系统中，commit 信息使用单引号 '，Windows 系统，commit 信息使用双引号 "。

所以在 git bash 中 git commit -m '提交说明' 这样是可以的，在 Windows 命令行中就要使用双引号 git commit -m "提交说明"。

git基本操作

git工作创建和保存项目快照及与之后的快照进行对比

![image](https://www.runoob.com/wp-content/uploads/2015/02/git-command.jpg)

local repository：版本库或本地仓库

remote repository：远程仓库

![image](https://remnote-user-data.s3.amazonaws.com/LmQZ_tWoWr-RtbG3XKh_S5vOS-KQBjioCtb9hupjO4pnJyjJkWrIe_oYi-_ywvejtFbPYdkgILQ_YKCphAxdziBbFKqKiDayVK-cIsF55ZYqj2K9-iSQ9-6suqYxd65M.png)

git 分支管理

使用分支将工作切分开来，从而让我们能够在不同开发环境中做事，并来回切换