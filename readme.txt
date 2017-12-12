git is a version control system
基础命令：
git init：					初始化创建一个仓库
git status：  				获取仓库的状态              
git add： 					添加到仓库，改变到即将提交的状态
git commit -m "desc"： 		提交修改
git log：  					查看版本信息
git log --pretty=oneline： 	查看库信息。在一行显示
git diff： 					查看不同，添加以后就看不出。
git reset --hard HEAD^： 	回退到上一个版本
git reset --hard 版本号： 	回退到指定的一个版本
git reflog： 				记录git的每一次命令
git checkout -- readme.txt：可以丢弃工作区的修改 (修改文件后还没有提交到暂存区)
git reset HEAD readme.txt： 可以让暂存区的东西回退到add前，然后就可以利用git checkout -- readme.txt 			 								丢弃工作区的修改~（已经add到暂存区，但是还没有commit提交到分支。)
git rm file4.txt:			删除一个文件
git remote add origin git@... 关联一个远程库
git push -u origin master 	第一次推送master分支的所有内容
git push origin master 		推送最新的修改
git clone 克隆一个仓库 （git 支持多种协议 包含合https和ssh,但是ssh的协议速度最快）

git branch 查看分支
git breanch [name] 创建分支
git checkout [name] 切换分支
git checkout -b [name] 创建加切换分支
git merge [name] 合并某分支到当前分支
git branch -d [name] 删除分支


工作区：电脑中所看到的目录，目录里的 .git 不算工作区，只是git的版本库
暂存区：add会把内容由工作区提交到暂存区，然后commit会把暂存区的内容提交到当前分支。
版本库：本地库和远端库
本地库：
远端库：

管理修改：如果修改不add到暂存区，就不会加入到commit中

add到暂存区后，让文件返回到未add的前的状态,然后就可以通过上面一行的命令丢弃工作区的修改了~
修改以后提交到了暂存区还提交到了本地库：git reset --hard HEAD^(返回上一个版本)
