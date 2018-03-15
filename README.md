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

### 关联远程分支

关联之后，git branch -vv就可以展示关联的远程分支名了，同时推送到远程仓库直接：git push，不需要指定远程仓库了。

```
$ git branch -u origin/mybranch
```
或者在push时加上-u参数

```
$ git push origin/mybranch -u
```








