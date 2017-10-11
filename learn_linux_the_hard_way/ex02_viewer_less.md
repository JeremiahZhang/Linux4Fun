# 第二章: Text Viewer

> `less` is `more`

more 也是一个查看器, 非常简单.

后来, Mark Nudelman 在1983-1985年写了个 `less`, 里面有好多功能.

## 实战

Type in terminal

```
less .bashrc
```

outputs:

```
# ~/.bashrc: executed by bash(1) for non-login shells.
# see /usr/share/doc/bash/examples/startup-files (in the package bash-doc)
# for examples

# If not running interactively, don't do anything
case $- in
    *i*) ;;
      *) return;;
esac

# don't put duplicate lines or lines starting with space in the history.
# See bash(1) for more options
HISTCONTROL=ignoreboth

```

## 快捷键

使用less的基本快捷键和vim有类似之处:

- `j` -- move up
- `k` -- move down
- `q` -- quit `less`
- `--chop-long-lines` or `--ch<Enter><Enter>`: type `--ch` 再按两次回车, 
    - 该功能是将一长行, 无法在terminal 屏幕上一次显示, 将其能一次在该屏幕上显示
    - 也就是一行非常长, 可多行在terminal的屏幕上显示
- `/` -- search
- `&something` -- show only those line from your file which contain `something`.
    - 再次type, `&<ENTER>` 则回到先前的整个文档模式.

## end

本次学习文本查看器`less`的最基础功能. 新技能get!

```
@jeremy_anifacc
2017-10-11
```
