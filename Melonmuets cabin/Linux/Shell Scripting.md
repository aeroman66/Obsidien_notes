# Variables
```shell
foo=bar
echo $foo

//定义string的几种方式
echo "World"
echo 'World'
echo "Value is $foo"
echo 'Valus is $foo'
```
	注意不能加空格，以及最后两种定义string的方式是不一样的。

# Functions
## Vim
	所有的Unix like系统都会内置vi文书编辑器。vim很常用。
```shell
vim mcd.sh
```

## 执行
```shell
mcd(){
	mkdir -p "$1"
	cd "$1"
}

source mcd.sh
mcd test
```

```shell
$?  //返回错误代码
$_  //返回最近巴拉巴拉（不懂）
$0 name of the script we are running
$# the number of arguments we are giving
$$ the process ID of this command that is running
$@ all the arguments we give
```

## Debug
```shell
shellcheck
```
# 逻辑运算符
||
&&
; : 仅仅是用于连接两个命令

# Getting the Output of a Command into a Variable
```shell
foo=$(pwd)

cat <(ls) <(ls ..) //可能把两个目录合并起来了
```

# E.g
```shell
#!/bin/bash

echo "Starting program at $(date)"

echo "Running program $0 with $# arguments with pid $$"

for file in "$@";do
	grep foobar "$file" > /dev/null 2>/dev/null

	if [["$? -ne 0"]];then
		echo "File $file does not have any foobar,adding one"
		echo "# foobar" >> "$file"
	fi

done
```

# Globbing
```shell
ls *.sh*
```
	project1 project2 project42
		? will only expend to one character.
		以下的代码就只会打印project1和project2
```shell
ls project?
```
```shell
convert image.jpg image.png
convert image.{jpg,png}

touch foo{,1,2,10}
touch {foo bar}/{a..j}
```

# Shebang
	shell内置了很多语言，，都可以用vim在里面编辑
	第一行是告诉shell这个程序应该怎么执行的
```python
#!/usr/local/bin/python
import sys
for arg in reversed(sys.argv[1:]):
	print(arg)
```
	然而有时候我们并不知道解释器的具体位置在哪里，于是我们可以像下面这么做。
	shell就会在这个目录下找python这个可执行文件。
	这样还可以增强程序的可移植性。
```python
#!/usr/bin/env python
```

# 一些有用的工具
	比较琐碎还是得想想怎么学习。

评价是不如直接去学给的笔记。
## 查找
### 文件
### 命令
```shell
history

history 1| grep convert
```
ctrl+R