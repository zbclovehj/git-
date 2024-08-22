# git

所有的配置文件，其实都保存在本地！
查看配置git config -l
#查看系统config   				 git config --system --list　
#查看当前用户（global）配置		git config --global  --list

当你安装Git后首先要做的事情是设置你的用户名称和e-mail地址。这是非常重要的，因为每次Git提交都会使用该信息。它被永远的嵌入到了你的提交中：

git config --global user.name "****"  #名称
git config --global user.email ******@qq.com   #邮箱

Git本地有三个工作区域：工作目录（Working Directory）、暂存区(Stage/Index)、资源库(Repository或Git Directory)。


创建仓库 git init 或者 git clone 远程仓库
仓库中的文件初始状态都是未跟踪的

#查看指定文件状态
git status [filename]

查看所有文件状态

git status   获得状态

git add .                添加所有文件到暂存区、


git commit -m "消息内容"  提交暂存区中的内容到本地仓库 -m 提交信息

git push origin master 这里表示将本地仓库当前master分支的内容推到远程仓库上面去
# 列出所有本地分支
git branch
# 列出所有远程分支
git branch -r
# 新建一个分支，但依然停留在当前分支
git branch [branch-name]
# 新建一个分支，并切换到该分支
git checkout -b [branch]
# 合并指定分支到当前分支
$ git merge [branch]
# 删除分支
$ git branch -d [branch-name]
# 删除远程分支
$ git push origin --delete [branch-name]
$ git branch -dr [remote/branch]


