# Exercise 1 Text Editor: vim

> In linux, everything is just a file.

> Unix philosophy states that configuration files must be human readable and editable. In almost all cases, they are just plain text. 

We must learn how to edit a text file.

## Basics of vim

```
$touch hello.txt

$vim hello.txt
```

- Modes of vim
   - NORMAL: 
       - moving your cursor around
       - doing operations with text like delete, copy and paste.
   - INSERT:
       - entering text

> List of commands to navigate the cursor in NORMAL mode

- `h`- move left
- `j`- move down
- `k`- move up
- `l`- move right
- `i`- enter INSERT mode
- `o`- insert a line under cursor and enter `INSERT` mode
- `esc`- exit `INSERT` mode
- `x`- delete symbol under cursor
- `dd`- delete a line
- `:wq` - write changes to the file and exit.
- `:q!` - do not write changes to the file and exit.

`h`, `j`, `k`, `l` 正好在一起. 多使用就知道了. 不用特别去记忆. 用的时候记一下就可以了.

## ChangeLog

```
@Jeremy_Anifacc
2017.10.09 Discover + vim-adventrues.com 0:56
```
