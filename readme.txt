git init  //把目录变成git可以管理的仓库
git add -- readme.txt  //把readme.txt文件添加到仓库（文件要放在git可以管理的目录下）
git commit -m "这里是提交说明"  //把文件提交到仓库
git status  //查看被修改的文件
git diff  //查看修改内容
git diff HEAD -- readme.txt  //查看readme.txt工作区和版本库里最新版本的区别
git log  //查看提交历史（head是当前版本）
git log --pretty=oneline  //仅显示版本号和说明
git reset --hard HEAD^  //回退到上一个版本，HEAD^^为上上个版本，HEAD~100为上100个版本
git reset --hard + commit_id（版本号） //版本号没必要写全，前几位就可以，git会自动去找（前5位即可）
git reflog  //查看命令历史，可以查看回退前版本号
git checkout -- readme.txt //把readme.txt文件在工作区的修改全部撤销，这里有两种情况：
						   //一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
					       //一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
git reset HEAD readme.txt  //可以把readme.txt在暂存区的修改撤销掉，重新放回工作区
git rm test.txt  //从版本库中删除test.txt文件，并且要执行git commit

git remote add origin git@github.com:xiehongtao1224/learngit.git  //关联xiehongtao1224/learngit.git的远程库
git push -u origin master  //第一次推送master分支的所有内容到远程库
git push origin master  //第一次之后，推送最新修改到远程库
git clone git@github.com:xiehongtao1224/learngit.git  //克隆xiehongtao1224/learngit.git远程库到本地
git branch  //查看分支
git branch <name>  //创建分支
git checkout <name>  //切换分支
git checkout -b <name>  //创建+切换分支
git merge <name>  //合并某分支到当前分支
git branch -d <name>  //删除分支

Creating a new branch is quick and simple.

