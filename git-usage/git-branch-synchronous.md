## 同步问题 场景划分
### 场景一 已经创建本地分支A，但是远程没有此分支A
```sequence
title: 方法一
participant repository/git directory(资源库) as rpt
participant remote(git仓库) as rmt
rpt -> rmt : (1) git push --set-upstream origin remote-new-branch
```

```sequence
title: 方法二
participant repository/git directory(资源库) as rpt
participant remote(git仓库) as rmt
rpt -> rmt : (1) git push origin remote-new-branch:local-branch
```
### 场景二 远程存在分支A，但是本地没有分支A
```sequence
participant worksapce(工作区) as wk
participant index/stage(暂存区) as idx
participant repository/git directory(资源库) as rpt
participant remote(git仓库) as rmt
```
### 场景三 本地删除分支A，但是远程没有分支A

## Reference
[git仓库同步问题](https://www.php.cn/blog/detail/24922.html)