+ 建git库  git init
+ 添加到暂存区(stage) git add 文件 或 git add -A
+ 提交暂存区修改到新版本 git commit -m '提交日志'
+ 显示提交日志,可以查看到commit id，修改日期，修改人等
'git log
git log --pretty=oneline'
+ 撤销文件修改 git checkout --file 将文件恢复到最近的commit或add状态
+ unstage撤销  git reset HEAD file
----
+ 远程仓库关联有ssh key相关问题
+ 远程仓库关联 git remote add origin https://github.com/littleclaw
+ 推代码,第一次建立关联要加-u  git push -u origin master
+ 克隆远程库到本地 git clone gitURL
--------
+ 分支  查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>

