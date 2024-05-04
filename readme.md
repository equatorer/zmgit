# 1. 本地操作
1. 利用`~\.bashrc`修改git终端长命令，比如`git-log`、`ll`;
1. `git reset --hard commitid`回退版本，`git reflog`查找所有版本历史;
1. `git checkout branchid`是切换分支;
1. 当有冲突时，先人工处理冲突，然后add，最后commit;
1. 没有merge的分支，可以用`git branch -D branchid`删除;
1. `git restore --staged .`可以将上次所有`add`的内容撤销，如果有`.gitignore`则只取消其不忽视的文件;
# 2. 远程操作
1. `git remote add remoteid remoteurl`添加远程地址;
1. `git push remoteid branchid`推送本地branchid至远程remoteid;
1. `git brach -vv`查看分支更多信息
1. `git clone sshurl id.git`克隆远程仓库到本地并以特有id为git库;
1. `git fetch`抓取置零就是将仓库里的更新都抓取到本地，但不进行合并;
1. `git pull`拉取指令就是将远端仓库的修改拉到本地并自动进行合并，相当于`fetch+merge`;
1. 解决远程冲突就是先`fetch+merge`或`pull`，修改完冲突后再`push`;
1. 