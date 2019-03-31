# GitHub 

## 入门

### 课程目标

#### 实名注册GitHub账户

#### 点亮个人头像

#### 完善个人资料

#### 能够在GitHub上搜索资料

##### 搜索人

##### 搜索项目

#### 能够评估人和项目的活跃度

#### 掌握GitHub社交化

##### star   收藏项目

##### follow 关注高手

#### 能够创建/删除GitHub远程仓库

#### 能够建立本地仓库

#### 能够把本地仓库和远程仓库建立关联

#### 能够在本地仓库和远程仓库之间pull（推上去）和push（拉下来）

### 开源社区

#### GitHub（全世界最大的开源社区）

#### SourceForge

#### Google code

#### codeplex

#### 开源中国

## git bush 

### git bash命令

#### bash  命令体验

##### # change directory     cd

###### 改变目录

##### # make directory   mkdir

###### 创建目录

##### # print working directory   pwd

###### 打印当前工作目录

##### # move  mv

###### 移动文件

##### # copy cp

###### 复制

##### # remove  rm

###### 移动文件

#### 说明

##### workspace:工作区

##### index/stage:暂存区

##### Repository:仓库区（或本地仓库）

##### remote：远程仓库，例如：GitHub

#### 新建代码仓库命令

##### git init

###### 在当前目录新建一个Git代码库

##### git clone[url]

###### 下载一个项目和她的整个代码历史

###### URL格式：https://github.com/[UserName]/reposName

#### 添加删除文件

##### git add [file1] [file2]

###### 添加指定文件到暂存区

##### git rm [file1] [file2]

###### 删除工作区文件，并且将这次删除放入暂存区

##### git mv [file-origin] [file-renamed]

###### 改名文件，并且将这个改名放入暂存区

#### 代码提交

##### git commit -m [message备注]

###### 提交暂存区到仓库

##### git commit -a -m [message]

###### 直接从工作区提交到仓库，前提该文件已经有仓库中的历史版本

#### 查看信息

##### git status

###### 显示变更信息

##### git log   git log --oneline

###### 显示当前分支的历史版本

#### 同步远程仓库

##### git remote add [shortname]  [url]

###### 增加远程仓库，并命名

##### git push [remote] [branch]

###### 将本地的提交推送到远程仓库

##### git pull [remote] [branch]

###### 将远程仓库的提交拉下到本地

#### 遇到一些问题

##### 命令行换行

###### 错误的输入“\”换行符，这个时候命令并不退出，只是换到下一行，多了一个>，这并不影响操作 可以继续执行命令。

##### 命令行终结

###### Ctrl+c 强制退出

##### 命令行翻页和退出   git log

###### 下/上翻页：Ctrl+u

###### 退出：q或者Ctrl+c

###### 最上：gg

###### 最下：G

###### 搜索：/n

###### 下一匹配项：u

###### 上一匹配项：

##### vim的模式操作

###### 编辑模式

####### i

###### 回到普通模式

####### Esc

###### 保存退出

####### wq
