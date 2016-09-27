Git is a version control system.
Git is free software.
初始化一个Git仓库，使用git init命令。
添加文件到Git仓库，分两步：
第一步，使用命令git add <file>，注意，可反复多次使用，添加多个文件；
第二步，使用命令git commit，完成。
mkdir learn git
cd learn git 
pwd
git reflog
git add XXX.txt
git commit -m "XXX"
git log
git diff
第一步是用git add把文件添加进去，实际上就是把文件修改添加到暂存区；

第二步是用git commit提交更改，实际上就是把暂存区的所有内容提交到当前分支。

因为我们创建Git版本库时，Git自动为我们创建了唯一一个master分支，所以，现在，git commit就是往master分支上提交更改。

你可以简单理解为，需要提交的文件修改通通放到暂存区，
一次性提交暂存区的所有修改。
git checkout命令加上-b参数表示创建并切换，相当于以下两条命令：

$ git branch dev
$ git checkout dev
Switched to branch 'dev'