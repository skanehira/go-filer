# ff
`ff` is file manager written in Go.

![](https://i.imgur.com/ZAKJfdC.gif)

# Features
- preview file/directory
- copy/paste file
- make a new file/directory
- rename a file/directory
- edit file with `$EDITOR`
- open file/directory

# Support OS
- Linux
- Mac

# Installtion
```sh
$ git clone https://github.com/skanehira/ff
$ cd ff
$ go install
```

NOTE: Installation with `go get` is not recommended because libraries is not version locked.

# Usage
## Settings
If your terminal `LC_CTYPE` is not `en_US.UTF-8`, please set as following.

```sh
export LC_CTYPE=en_US.UTF-8
```

## Options
```sh
$ ff -h
Usage of ff:
  -log
        enable log
  -preview
        enable preview panel
```

If you use `-log` that will print log. If log file not exists then will be create in `$HONE/ff.log`.

`-preview` is enable preview panel that you can preview file or directories.

## About open action
If you use `o` to open something, ff will using `open` in MacOS, `xdg-open` in Linux.

## Keybinding
| panel | key      | operation                            |
|-------|----------|--------------------------------------|
| path  | `tab`    | focus to files                       |
| files | `tab`    | focus to path                        |
| files | `j`      | move to next                         |
| files | `k`      | move to previous                     |
| files | `g`      | move to top                          |
| files | `G`      | move to bottom                       |
| files | `ctrl-b` | move previous page                   |
| files | `ctrl-f` | move netxt page                      |
| files | `h`      | cd to specified path                 |
| files | `l`      | cd to parent path                    |
| files | `y`      | copy selected file                   |
| files | `p`      | paste copy file to current directory |
| files | `d`      | delete selected file or directory    |
| files | `m`      | make a new dir                       |
| files | `n`      | make a new file                      |
| files | `r`      | rename a dir or file                 |
| files | `e`      | edit file with `$EDITOR`             |
| files | `o`      | open file or directory               |
| files | `f`/`/`  | search files or directories          |
| files | `ctrl-j` | scroll preview panel down            |
| files | `ctrl-k` | scroll preview panel up              |

# Author
skanehira
