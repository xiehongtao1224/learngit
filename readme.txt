git init //把目录变成git可以管理的仓库
git add -- readme.txt //把readme.txt文件添加到仓库（文件要放在git可以管理的目录下）
git commit -m "这里是提交说明" //把文件提交到仓库
git status //查看被修改的文件
git diff //查看修改内容
git diff HEAD -- readme.txt //查看readme.txt工作区和版本库里最新版本的区别
git log //查看提交历史（head是当前版本）
git log --pretty=oneline //仅显示版本号和说明
git reset --hard HEAD^ //回退到上一个版本，HEAD^^为上上个版本，HEAD~100为上100个版本
git reset --hard + commit_id（版本号） //版本号没必要写全，前几位就可以，git会自动去找（前5位即可）
git reflog //查看命令历史，可以查看回退前版本号
git checkout -- readme.txt //把readme.txt文件在工作区的修改全部撤销，这里有两种情况：
						   //一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
					       //一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
git reset HEAD readme.txt //可以把readme.txt在暂存区的修改撤销掉，重新放回工作区