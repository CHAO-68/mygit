# 1、git入门简介
1、创建新仓库
`git init`

2、工作流
![image](https://user-images.githubusercontent.com/63992601/141035088-69c13f1b-73db-40be-ab3e-d6b183fd6e73.png)

3、添加和提交
- 你可以提出更改（把它们添加到暂存区），使用如下命令：
  `git add <filename>`
  
  `git add *`
- 这是 git 基本工作流程的第一步；使用如下命令以实际提交改动：
  `git commit -m "代码提交信息"`
  
4、推送改动
- 你的改动现在已经在本地仓库的 HEAD 中了。执行如下命令以将这些改动提交到远端仓库：
`git push origin master`
可以把 master 换成你想要推送的任何分支。

- 如果你还没有克隆现有仓库，并欲将你的仓库连接到某个远程服务器，你可以使用如下命令添加：
`git remote add origin <server>`
如此你就能够将你的改动推送到所添加的服务器上去了。
