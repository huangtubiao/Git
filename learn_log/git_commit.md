# git commit 指令
* [参考资料](https://www.kernel.org/pub/software/scm/git/docs/git-commit.html)
* [参考资料2](https://git-scm.com/docs/git-commit)
* `git commit -am` 相当于`git commit -a -m`
* `git commit -a`
	* Tell the command to automatically stage files that have been modified and deleted, but new files you have not told Git about are not affected.
	* 该指令将**修改**或**删除**的改动放入暂存区，注意**新文件**不会放入暂存区；
* `git commit -m`
	* Use the given <msg> as the commit message. If multiple -m options are given, their values are concatenated as separate paragraphs.
	* 该指令将暂存区的改动放入本地仓库（当前分支），如果使用了多个“-m”则会将该提交分成多个段落显示；例如： 使用了`git commit -m "格式统一化" -m "多个注释会怎样？"` gitHub上会这样显示：
	* ![多行-m的截图](https://github.com/huangtubiao/Git/blob/master/learn_log/log_img/git_commit_s1.png)

## git commit 常用指令：
* git commit -am "注释内容"
  * 将 **工作区** 以及 **暂存区** 代码放入 **本地仓库**（不包括**工作区**新建的文件）
  * `git add -A`将所有 **工作区** 代码放入 **暂存区**（包括**新建**的文件）

* git commit -m "注释内容"
  * 将 **暂存区** 代码放入 **本地仓库**
  
* git commit --amend 
  * 可以对上一次的提交做修改

### git commit message:
- [Git Commit Log 的小型团队最佳实践](https://mp.weixin.qq.com/s/iaiejkugOqV4rg2hXuHOAw)
- [优雅地提交你的 Git commit message](https://juejin.im/post/5afc5242f265da0b7f44bee4) 
- [An emoji guide for your commit messages](https://gitmoji.carloscuesta.me/)

## 相关指令：
* [git_status.md](https://github.com/huangtubiao/Git/blob/master/learn_log/git_status.md)  查看当前代码状态指令： 提交代码到**本地仓库**后， 用我可以查看有多少个commit等待提交到远程哦！

* [git_push.md](https://github.com/huangtubiao/Git/master/learn_log/git_push.md) 提交代码至远程仓库指令： `git commit`后， 接下来就是我`git push`出场了！
