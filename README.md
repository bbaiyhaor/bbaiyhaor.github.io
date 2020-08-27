# bbaiyhaor.github.io

# chmod 命令：chmod ［mode］ 文件名

-rw-r--r--，共有10个位置，第一个字符指定了文件类型。如果第一个字符是横线，表示是一个非目录的文件。如果是d，表示是一个目录。
从第二个字符开始到第十个共9个字符，3个字符一组，分别表示了3组用户对文件或者目录的权限。
权限字符用横线代表空许可，r代表只读，w代表写，x代表可执行。
数字与字符对应关系如下：
r=4，w=2，x=1
若要rwx属性则4+2+1=7
若要rw-属性则4+2=6；
若要r-x属性则4+1=7。

命令：chmod 751 file  

说明：给file的属主分配读、写、执行(7)的权限，给file的所在组分配读、执行(5)的权限，给其他用户分配执行(1)的权限

# kill 命令：

kill -9 pid 强制kill掉pid进程

# ps(process status)命令：

ps aux/ps -ef 查看所有进程状态

# git把一个commit分成多个commit

git rebase -i <commit-hash>~或者git rebase -i <hash-of-previous-commit>

在vim编辑页面中找到要更改的那次commit，将其前面的 pick 改成 edit，保存退出vim

git reset HEAD~ 回退到上一次提交

若干次提交：

  ```
  git add files

  git commit -m "第i个commit"
  ```
  
git rebase --continue
 


