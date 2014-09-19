git config --global user.name "xingke"
git config --global user.name "xingkongyingke@163.com"
mkdir learngit
cd learngit
pwd
git init
git add readme.txt
git commit -m "wrote a readme file"
git status
git diff readme.txt
git log    //命令显示从最近到最远的提交日志
git log --pretty=oneline  //简化显示日志
git reset --hard HEAD^    //回退到上一个版本
git reset --hard 3628164   //回退到指定版本，数字可以省略一部分
git reflog
rm test.txt    //删除文件

git rm test.txt  //从git中删除
git commit -m "remove test.txt" //提交删除

git checkout -- test.txt  //回复文件

ssh-keygen -t rsa -C "xingkongyingke@163.com"   //生存自己的密钥   提示输入信息不要输入：输入回有问题：记住直接下一步
git remote add origin git@github.com:xingkongyingke/learngit.git  //绑定上github
git push -u origin master     //推送上传  第一次用要加 -u
git push origin master   //以后直接推送

git clone git@github.com:xingkongyingke/learngit.git

git checkout -b dev  //创建dev分支, 可拆分为下面两条
git branch dev
git checkout dev 

git branch   //列处当前所有的分支
git checkout master //切换到master分支
git merge dev    //把dev分支合并到master分支上

