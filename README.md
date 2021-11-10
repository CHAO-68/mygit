# 1、git入门简介

1、创建新仓库 `git init`

2、工作流 [![image](https://user-images.githubusercontent.com/63992601/141035088-69c13f1b-73db-40be-ab3e-d6b183fd6e73.png)](https://user-images.githubusercontent.com/63992601/141035088-69c13f1b-73db-40be-ab3e-d6b183fd6e73.png)

3、添加和提交

- 你可以提出更改（把它们添加到暂存区），使用如下命令： `git add <filename>`

  `git add *`

- 这是 git 基本工作流程的第一步；使用如下命令以实际提交改动： `git commit -m "代码提交信息"`

4、推送改动

- 你的改动现在已经在本地仓库的 HEAD 中了。执行如下命令以将这些改动提交到远端仓库： 

  `git push origin master` 可以把 master 换成你想要推送的任何分支。

- 如果你还没有克隆现有仓库，并欲将你的仓库连接到某个远程服务器，你可以使用如下命令添加：

   `git remote add origin <server>` 如此你就能够将你的改动推送到所添加的服务器上去了。

5、分支

分支是用来将特性开发绝缘开来的。在你创建仓库的时候，*master* 是“默认的”分支。在其他分支上进行开发，完成后再将它们合并到主分支上。

- 创建并切换分支

  `git checkout -b feature_x`

- 切换回主分支：

  `git branch checkout master`

- 创建新的分支

  `git branch b`

- 查看当前在哪个分支

  `git status`

- 删除分支

  `git branch -d a`

- 将本地仓库的head提交到远程仓库（选择分支）

  `git push origin master`

6、更新与合并

- 要更新你的本地仓库至最新改动，执行：

  `git pull`

- 要合并其他分支到你的当前分支（例如 master），执行：

  `git merge <branch>`

- 在这两种情况下，git 都会尝试去自动合并改动。遗憾的是，这可能并非每次都成功，并可能出现*冲突（conflicts）*。 这时候就需要你修改这些文件来手动合并这些*冲突（conflicts）*。改完之后，你需要执行如下命令以将它们标记为合并成功：

  `git add <filename>`

- 在合并改动之前，你可以使用如下命令预览差异：

  `git diff <source_branch> <target_branch>`

7、标签

`git tag 1.0.0 1b2e1d63ff`

`git log`

8、替换本地改动

- 你可以使用如下命令替换掉本地改动：

  `git checkout -- <filename>`

​	此命令会使用    HEAD 中的最新内容替换掉你的工作目录中的文件。已添加到暂存区的改动以及新文件都不会受到影响。

- 假如你想丢弃你在本地的所有改动与提交，可以到服务器上获取最新的版本历史，并将你本地主分支指向它：

  `git fetch origin`

  `git reset --hard origin/master`

9、删除文件

- 如果你想从资源库中删除文件，我们使用rm。

​	`git rm file`

# 2、git基本操作汇总

![image-20211110121233254](C:\Users\86156\AppData\Roaming\Typora\typora-user-images\image-20211110121233254.png)

![image-20211110121302315](C:\Users\86156\AppData\Roaming\Typora\typora-user-images\image-20211110121302315.png)

