git is a version control system
基础命令：
git init 初始化创建一个仓库
git status  获取仓库的状态              
git add 添加到仓库，改变到即将提交的状态
git commit -m "desc" 提交修改
git log  查看版本信息
git reflog 记录git的每一次命令
git diff 查看不同

工作区，暂存区
版本库，远端库

删除一次修改
修改以后没有提交到暂存区:git checkout -- readme.txt 丢弃工作区的修改
修改以后提交到了暂存区：git reset HEAD readme.txt add到暂存区后，让文件返回到未add的前的状态,然后就可以通过上面一行的命令丢弃工作区的修改了~
修改以后提交到了暂存区还提交到了本地库：git reset --hard HEAD^(返回上一个版本)
