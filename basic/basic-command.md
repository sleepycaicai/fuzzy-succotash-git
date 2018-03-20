## 常用的 git 命令及解释

git init： 在当前目录下初始化一个 git 仓库

git add filename: 将名为filename的文件加入 git 的版本控制下

git commit -m "message": 提交项目的更改

git clone remote-path: 远程克隆一个仓库到本地

git push origin master: 将当前的 master 分支推送到远程仓库

git checkout -b test： 创建一个名为 test 的新分支，并且切换到新分支下

git push origin test: 推送 test 分支到远程仓库，会在远程仓库创建一个名为 test 的分支

git checkout master: 切换到 master 分支

git merge test: 合并 test 分支到 master 分支

git branch -d test: 删除 test 分支

git push origin :test : 删除远程仓库中的 test 分支。 这是因为完整的命令形式是 git push remote-name local-brabch:remote-branch, 这里local-branch 为空，就意味着推送一个空到remote-branch, 也就是删除了 remote-branch

git tag "V1.0" 为当前提交打标签

git push origin master --tags: 推送时默认不会带有tag, 需添加参数 --tags

git fetch origin hello:hello : git拉取远程仓库的特定分支到本地 remote-branch-name:local-branch-name, 此种方式本地 hello 分支不会自动和远程分支 hello 建立关系

git push origin hello:hello : 推送本地hello分支的更新到远程的hello分支，完整命令形式git push remote-name local-brabch:remote-branch


