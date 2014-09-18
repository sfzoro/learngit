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
