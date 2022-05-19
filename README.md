# Git practice and leetcode practice

## git workflow command
```sequence
title: git workflow command
participant worksapce(工作区) as wk
participant index/stage(暂存区) as idx
participant repository/git directory(资源库) as rpt
participant remote(git仓库) as rmt

rmt -> wk : pull 从远端拉分支到工作区（对象当前分支）
rmt -> rpt : fetch/clone 从远端仓库拷贝仓库到本地仓库
rpt -> rmt : push 从本地仓库推送到远端仓库
rpt -> wk : checkout 从本地仓库选择工作分支到工作区域
wk -> idx : add 从工作区域添加修改到暂存区
idx -> rpt : commit 从暂存区提交到本地仓库
```

## markdown grammer
### sequence grammer
![时序图语法](https://upload-images.jianshu.io/upload_images/3830893-9f78bc169040ec84.png?imageMogr2/auto-orient/strip|imageView2/2/w/709/format/webp)