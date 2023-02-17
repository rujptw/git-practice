# git 常用命令

  1. git log: 打印提交纪录,加上--graph --oneline 参数可以较为美观地打印出log
  2. git init: 初始化git仓库
  3. git add: 将文件变更添加到索引中
  4. git commit:提交变更到本地仓库
  5. git clone：克隆远程仓库到本地
  6. git pull: 拉取远程仓库变更到本地
  7. git push: 推送本地仓库到远程仓库，-f:可以强制推送，覆盖远程仓库
  8. git reset hash值 --hard:强制重置索引，并取消所有变更
  9. git 命令 --help:弹出命令帮助文档
  10. git remote add [name] [url],添加远程仓库地址，name一般是origin，url是远程仓库地址
  11. git config --global push.autoSetupRemote true,当本地分支没有关联远程分支时，推送时默认关联远程默认分支，就不用使用git push --set-upstream origin master，每次都需要手动去关联。
  12. git branch 分支名,基于某个分支，创建一个新分支
  13. git branch -d 分支名,删除该分支
  14. git checkout 分支名,切换到该分支
  15. git checkout -b 创建一个新分支，并切换到该分支
  16. git stash,保存一个分支上在索引或者工作树上的工作，切换到另外一个分支，可以使用 pop或者apply参数还原工作。pop会删除缓存的stash，apply则不会
  17. 合并分支
      1. git merge 分支A 分支B,将分支B合并到分支B上，会保留修改内容的历史记录，形式一颗提交树，merge会比较清晰，详细
      2. git rebase，提交记录是线性的，也就是一根直线，会在原有提交的基础上将差异内容反应进去，有可能导致原有的内容提交内容无法正常运行，rebase的提交纪录则会比较简单
      3. git reset --hard HEAD~，取消最近的合并
   18. 
