# 二十九、GIT

## 1.初始化

git config --global user.name flk30rst					            	设置用户签名 

git config --global user.email flk30rst@163.com 			 		设置用户签名 

**git init** 														初始化本地库 

ll  -a



------

## 2.暂存库

git  status 													    查看本地库状态 

git  add   hi.txt       							  				    添加到暂存区 

git  rm  --cached   hello.txt  									      从暂存区删除 

git  commit    -m     "first commit"   hi.txt							提交到本地库 

git  reflog							     						 查看历史记录 

git  log							     						      查看历史记录

**git  reset --hard d504f2a**									          版本穿梭



------

## 3.分支

git branch -v 											    查看分支 

git branch hot-fix										     创建分支 

git checkout hot-fix	 									切换分支 

git checkout master										切换回去

git merge hot-fix  										    把指定的分支合并到当前分支上

ssh-keygen  -t  rsa  -C  flk30rst@163.com					    免密设置



------

## 4.远程库

查看当前所有远程地址别名 

git remote -v 



起别名

git remote add git-demo https://github.com/flk30rst/git-demo.git 



## 5.push

推送本地分支上的内容到远程仓库 

git push git-demo master



## 6.clone

将远程仓库的内容克隆到本地 

git clone https://github.com/flk30rst/git-demo.git 



## 7.pull

将远程仓库对于分支最新内容拉下来后与当前本地分支直接合并

git pull git-demo master