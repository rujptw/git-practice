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
