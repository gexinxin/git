# Git 进阶

## Git GUI

### 工具

#### git

#### EGit

#### GI+

### 指令

#### git reset HEAD

##### 回到仓库页面最后一条记录的投指针

### git 配置

#### 忽略一些内容：gitignore

##### vim .gitignore指令 然后进行纯文本编辑

###### 记得保存修改 并提交

##### 强制添加.gitignore忽略的文件

###### git add -f " file name"

##### 查看.gitignore策略生效行号

###### git check-ignore -v "file name"

### 别名

#### git log --pretty=format:'%h %ad | %s%d' --graph --date=short

##### 以图形的方式打印git提交日志

#### git config --global alias.ci commit

##### 设置别名

### 存储凭证

#### git config --global credential.helper wincred

### 本地协议

#### git clone /c/test/test.git（就是仓库的路径  .git可以省略）

##### 克隆本地仓库

#### it clone file:///c/test/test.git

##### 克隆本地仓库，不建议使用file://

#### git  remote add origin /c/teat/test.git

##### 添加远程仓库的链接

### git协议

#### git clone git://sever_ip/test.git

##### 克隆远程仓库

#### git remote add origin git://sever_ip/test.git

##### 添加远程仓库的链接

### HTTP协议

#### git clone https://github.com/gexinxin/test.git

##### 克隆远程仓库

#### git remote add origin https://github.com/gexinxin/test.git

##### 添加远程仓库的链接

### SSH协议

#### 克隆远程仓库，一般写成简短的命令

##### git clone git@github.com/gexinxin/test.git

##### git clone ssh://git@github.com/gexinxin/test.git

#### 添加远程仓库的链接

##### git remote add origin git@github.com/gexinxin/test.git

#### ssh-keygen -t rsa -C "your email"

##### 生成RSA密钥对

#### 在GitHub网站添加公钥

#### 使用SSH协议，克隆仓库或者添加远程链接

### git基本操作

#### git blame <file name>

##### 逐行查看文件的修改历史

#### git blame -L 100,10 <file name>

##### 从第100行开始，到底110行。装查看文件的修改历史

#### git

##### git 命令信息

#### git help -a

##### 查看全部的git子命令

#### git clean -n

##### 列出打算清除的档案

#### git clean -f

##### 真正的删除

#### git clean -x

##### 连 .gitignore中忽略的档案也删除

#### git add

##### touch a

###### 添加一个名字为a的新文件

##### git remote a

###### 删除文件a

##### echo  "增加的内容" >> a

###### 编辑文件a（增加内容）

#####  git mv a b

###### 文件改名  将a改为b

##### git mv a ./demo/

###### 将文件移动到demo库中

##### git add -p

###### 一个文件多个提交

##### git add.

###### 将文件夹内的所有操作都提交

#### git commit 

##### 一

###### git add .

###### git commit -m "message" 

##### 二

###### git commit -a -m "message" 

##### 三

###### git commit -am "message" 

#### 信息查看

##### git status -sb

###### short and branch

##### git show HEAD

###### 查看某个提交信息

##### 查看提交历史

###### git log <file name>

###### git log --grep <message>

###### git log -n

#### git diff

#### 回撤操作

只要不提交到远程仓库，怎么回撤都可以


##### git reset HEAD

###### 回撤暂存区内容到工作目录

##### git reset HEAD --soft

###### 回撤提交到暂存区

##### git reset HEAD -hard

###### 回撤提交，放弃变更

##### git push -f

###### 回撤远程仓库，-f就是-force

##### 回撤上一次提交

###### git add .

###### git commit --amend -m "message"

##### git rebase -i HEAD~3

###### 变基操作，改写历史提交

### 标签操作git tag

#### git tag foo

##### 在当前提交上，打标签foo

#### git tag foo -m "message"

##### 在当前提交上，打标签foo，并给message信息注释

#### git tag foo HEAD~4

##### 在当前提交之前的第4个版本上，打标签foo

#### git tag 

##### 列出所有标签

#### git tag -d foo

##### 删除标签

#### git push origin --tags

##### 表标签送到远程仓库

#### git push origin v0.1

##### 把标签推送到远程仓库

### 分支（*）

#### 冲突解决

##### 1. 在不同的分支上，修改同一个文件

##### 2. 不同的人，修改同一个文件

##### 3. 不同的仓库，修改同一个文件

##### 4. 冲突只在合并分支的时候才会出现

##### 5. 发生冲突并不可怕，冲突的代码不回丢失

##### 7.冲突信息的格式

#### 分支命令

##### git branch foo

###### 删除分支foo

##### git checkout foo

###### 切换到分支foo

##### git checkout -b foo

###### 删除分支并同时切换到foo，一部做到

##### 修改分支名称

###### git branch -m old_name new_name

###### git branch -M old_name new_name

##### 删除分支foo

###### git branch -d foo

###### git branch -D foo

##### 列出远程分支

###### git branch -r

##### 查看已合并的分支

###### git branch --merged

###### git branch --no-merged

##### 列出远程合并的分支

###### git branch -r --merged

##### 取出远程foo分支

###### git checkout -t origin/foo

##### 删除远程分支

###### git push origin <space>:<remote branch>

###### git fetch -p

##### 合并分支

###### git merge <branch name>

##### 合并分支，拒绝fast forward，产生合并commit

###### git merge --no-ff

#### git stash

##### git stash

###### 保存进度

##### git stash pop

###### 弹出进度

##### git stash list

###### 查看stash列表

##### git stash clear

###### 删除stash列表
