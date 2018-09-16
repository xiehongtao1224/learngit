git init //把目录变成git可以管理的仓库
git add //把文件添加到仓库（文件要放在git可以管理的目录下）
git commit -m "这里是提交说明" //把文件提交到仓库
git status //查看被修改的文件
git diff //查看修改内容
git diff HEAD -- readme.txt //查看工作区和版本库里最新版本的区别
git log //查看提交历史（head是当前版本）
git log --pretty=oneline //仅显示版本号和说明
git reset --hard HEAD^ //回退到上一个版本，HEAD^^为上上个版本，HEAD~100为上100个版本
git reset --hard + commit_id（版本号） //版本号没必要写全，前几位就可以，git会自动去找（前5位即可）
git reflog //查看命令历史，可以查看回退前版本号

