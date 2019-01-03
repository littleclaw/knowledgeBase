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
+ 拉代码 git pull <remote> <branch>
--------
### 分支  
+ 查看分支：git branch
+ 创建分支：git branch <name>
+ 切换分支：git checkout <name>
+ 创建+切换分支：git checkout -b <name>
+ 合并某分支到当前分支：git merge <name>
+ 删除分支：git branch -d <name>
	
--------

+ 把另一个分支代码合并到当前分支  git merge <name>

-----
###把所有改动暂存起来，回复到上一次提交状态 git stash

+ git stash pop 从暂时弹出上次暂存的改动
+ git stash list 列出栈元素
+ git stash apply stash@{0} 应用某个改动
+ git stash drop   删

-------
+ git rebase 对尚未推送或分享给别人的本地修改执行变基操作清理历史

+ git tag <tagName> 打标签
+ git tag 显示所有标签
+ git push origin <tagname>可以推送一个本地标签；
+ git push origin --tags可以推送全部未推送过的本地标签；
+ git tag -d <tagname>可以删除一个本地标签；
+ git push origin :refs/tags/<tagname>可以删除一个远程标签
-----
.gitignore 代码示例：
'
	# Windows:
	Thumbs.db
	ehthumbs.db
	Desktop.ini

	# Python:
	*.py[cod]
	*.so
	*.egg
	*.egg-info
	dist
	build

	# My configurations:
	db.ini
	deploy_key_rsa
'

### 将命令简化为别名 
+ git config --global alias.st status
+ git config --global alias.co checkout


