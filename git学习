cd .ssh 公钥
ssh-keygen -t rsa -C "youremail@example.com" 生成公钥私钥
ssh -T address

提交： git commit -a - m 'a"
git push -u origin master
git add ..
git clone 地址.... .git

git status 
git log //查看日志
git reflog  //
git diff a.txt

工作区 --> 暂存区 --> 版本库
git checkout -- readme.txt可以丢弃工作区的修改   //总之，就是让工作区的这个readme.txt文件回到最近一次git commit 或 git add时的状态
git reset HEAD readme.txt // 将readme.txt 提交到暂存区的退掉 清空暂存区
git restore readme.txt    //回退 提交到暂存区的修改。清空readme.txt提交到的暂存区 但是工作区的修改还没有修改
git reset --hard HEAD^ //版本回退


删除文件:先本地rm  再从版本库中删除该文件，git rm a.txt删掉，并且git commit
如果删错了 ：git checkout  -- a.txt     git checkout其实是用版本库里的版本替换工作区的版本，无论工作区是修改还是删除，都可以“一键还原”。

为本地仓库添加远程仓库：起名字叫origin
git remote add origin git@github.com:xiaoyuyefengkuang/githubTest.git

git push -u origin master //把本地仓库的master分支推送到远程仓库 
由于远程库是空的，我们第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。

删除远程库
如果添加的时候地址写错了，或者就是想删除远程库，可以用git remote rm <name>命令。使用前，建议先用git remote -v查看远程库信息：
$ git remote -v
