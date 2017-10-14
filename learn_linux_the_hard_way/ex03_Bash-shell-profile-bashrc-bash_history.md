# Exercise 3 Bash

`shell is also a program`.

`Bash`: `Bourne Again Shell`, which is in turn a pun.(双关).

```
1: ls -al
2: cat .profile
3: echo Hello, $LOGNAME!
4: cp -v .profile .profile.bak
5: echo 'echo Hello, $LOGNAME!' >> .profile
6: tail -n 5 .profile
7: history -w
8: ls -altr
9: cat .bash_history
10: exit
```

---

## learn

1. `ls -al`: prints out all file in current directory, including hidden ones.

```
-al
  a: all file list including hidden ones.
  l: long format

hidden file starts with dot .
```

2. `cat .profile`: prints out your `.profile` file.

3. `echo Hello, $LOGNAME!`: tell  shell, output a string **Hello, $LOGNAME!**, 其中 **$LOGNAME** 代表你的登录名. 我的是`anifacc`

4. `cp -v .profile .profile.bak`: 复制文件 `.profile` 到 `.profile.bak`, `-v` 表示 v(verbose)显示过程

5. `echo 'echo Hello, $LOGNAME!' >> .profile` : 将 string 'echo Hello, $LOGNAME' 写入 `.profile` 文件中.

6. `tail -n 5 .profile`: prints out exactly five lines from `.profile` file

7. `history -w` : 将所有命令行的记录写入 `.bash_history` file 中.

8. `ls -altr`: `-tr` means, file list is sorted by time in reverse direction.

9. `cat .bash_history`: prints out `.bash_history` file 中的内容.

10. 退出 shell.

---


## practice

```
anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ ls -al
total 24
drwxr-xr-x 2 anifacc anifacc 4096 Oct 14 14:53 .
drwxr-xr-x 4 anifacc anifacc 4096 Oct  9 21:23 ..
-rw-r--r-- 1 anifacc anifacc 1067 Oct  9 22:35 ex01_vim.md
-rw-r--r-- 1 anifacc anifacc 1269 Oct 11 19:25 ex02_viewer_less.md
-rw-r--r-- 1 anifacc anifacc 1244 Oct 14 14:53 ex03_Bash-shell-profile-bashrc-bash_history.md
-rw-r--r-- 1 anifacc anifacc   83 Oct 14 14:58 hello.txt


anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ cat hello.txt
Roses are red.
Violets are blue.
Linux is scary
But I'm scary too.

anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ echo hello $LOGNAME!
hello anifacc!

anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ echo 'hello linux4fun' >> hello.txt
anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ tail -n 3 hello.txtLinux is scary
But I'm scary too.
hello linux4fun

anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ ls -alt
total 24
-rw-r--r-- 1 anifacc anifacc   83 Oct 14 14:58 hello.txt
drwxr-xr-x 2 anifacc anifacc 4096 Oct 14 14:53 .
-rw-r--r-- 1 anifacc anifacc 1244 Oct 14 14:53 ex03_Bash-shell-profile-bashrc-bash_history.md
-rw-r--r-- 1 anifacc anifacc 1269 Oct 11 19:25 ex02_viewer_less.md
-rw-r--r-- 1 anifacc anifacc 1067 Oct  9 22:35 ex01_vim.md
drwxr-xr-x 4 anifacc anifacc 4096 Oct  9 21:23 ..

anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ cat hello.txt
Roses are red.
Violets are blue.
Linux is scary
But I'm scary too.
hello linux4fun

anifacc@mint ~/Documents/Linux4Fun/learn_linux_the_hard_way $ cp -v hello.txt hello.md
'hello.txt' -> 'hello.md'
```

## other

`toal BLOCKS`

> You can find the definition of that line in the `ls` documentation for your platform. For `coreutils ls` (the one found on a lot of Linux systems), the information can be found via `info coreutils ls`.

> For each directory that is listed, preface the files with a line `total BLOCKS`, where BLOCKS is the total disk allocation for all files in that directory.

`info coreutils ls`

`info coreutils`

看基本信息.
