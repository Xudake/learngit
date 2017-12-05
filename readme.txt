git is a version control system
基础命令：
git init 初始化创建一个仓库
git status  获取仓库的状态              
git add 添加到仓库，改变到即将提交的状态
git commit -m "desc" 提交修改
git log  查看版本信息
git log --pretty=oneline 查看库信息。在一行显示
git diff 查看不同，添加以后就看不出。
git reset --hard HEAD^ 回退到上一个版本
git reset --hard 版本号 回退到指定的一个版本
git reflog 记录git的每一次命令

工作区：电脑中所看到的目录，里面的目录 .git 不算工作区，只是git的版本库
暂存区：add会把内容由工作区提交到暂存区，然后commit把会把暂存区的内容提交到当前分支。
版本库，远端库

删除一次修改
修改以后没有提交到暂存区:git checkout -- readme.txt 丢弃工作区的修改
修改以后提交到了暂存区：git reset HEAD readme.txt add到暂存区后，让文件返回到未add的前的状态,然后就可以通过上面一行的命令丢弃工作区的修改了~
修改以后提交到了暂存区还提交到了本地库：git reset --hard HEAD^(返回上一个版本)
