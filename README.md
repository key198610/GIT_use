# GIT_use
使用记录  1212


目标文件夹:   
 git clone                             克隆项目到本地  
 git add '文件'                        添加提交的文件(暂存区)  
 git commit -m "提交信息"               提交信息描述  
 git remote add origin git地址         提交地址(第一次设置过后,后面不用设置,直接下一步提交到指定分支)   
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


// 
git pull   拉取最新远程分支  
git rebase (把自己的提交commit先取消，然后拉取pull最新远程分支)  
git diff   看见文件的修改    
git push -u origin master    (提交到那个分支)   


// 返回上次提交

01:上一次提交是HEAD^,上上次是HEAD^^,也可以写成HEAD～2 ,依次类推, 指将HEAD指针指到指定提交，历史记录中不会出现放弃的提交记录   
git reset --hard HEAD^     
git push origin master -f   

02: 是放弃指定提交的修改，但是会生成一次新的提交，需要填写提交注释，以前的历史记录都在；  
git revert HEAD  
git push origin master  

   
// 版本不同步 =>   
01: git pull origin 'git地址'   
02: git add README.md   
03:  push -u origin 分支     


// git添加所有新文件    
git add -A  提交所有变化    
git add -u  提交被修改(modified)和被删除(deleted)文件，不包括新文件(new)    
git add .   提交新文件(new)和被修改(modified)文件，不包括被删除(deleted)文件   
