# git-tips
 
## 概念: 
    
    * 工作区：改动（增删文件和内容）
    * 暂存区：输入命令：git add 改动的文件名，此次改动就放到了‘暂存区’
    * 本地仓库(简称：本地)：输入命令：git commit 此次修改的描述，此次改动就放到了’本地仓库’，每个commit，我叫它为一个‘版本’。
    * 远程仓库(简称：远程)：输入命令：git push 远程仓库，此次改动就放到了‘远程仓库’（GitHub等)
    * commit-id：输出命令：git log，最上面那行commit xxxxxx，后面的字符串就是commit-id
 
### help

```
$ git help
```

### 抛弃本地所有的修改，回到远程仓库的状态。

```
$ git fetch --all && git reset --hard origin/master
```

### 列出所有远程分支

-r参数相当于：remote

```
$ git branch -r
```

### 列出本地和远程分支

-a参数相当于：all

```
$ git branch -a
```

### 创建并切换到本地分支 `git checkout -b <branch-name>`
### 创建并切换到远程分支 `git checkout -b <branch-name> origin/<branch-name>`
### 删除本地分支 `git branch -d <local-branchname>`
### 删除远程分支 `git push origin --delete <remote-branchname>` 或者 `git push origin :<remote-branchname>`
### 重命名本地分支 `git branch -m <new-branch-name>`
### 查看标签 `git tag` 展示当前分支的最近的tag `git describe --tags --abbrev=0`
### 本地创建标签 `git tag <version-number>` 默认tag是打在最近的一次commit上，如果需要指定commit打tag：`git tag -a <version-number> -m "v1.0 发布(描述)" <commit-id>`



















