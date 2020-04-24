# GIT_use
使用记录


目标文件夹: 
 git clone                             克隆项目到本地
 git add '文件'                        添加提交的文件
 git commit -m "提交信息"              提交信息描述
 git remote add origin git地址         提交地址
 git push -u origin master(分支)       提交分支


// master => 开发分支
git checkout master 
git pull 
git checkout 开发分支
git merge master 
git push -u origin 开发分支


// 开发分支 => master
git checkout 开发分支
git pull
git checkout master
git merge 开发分支
git push -u origin master