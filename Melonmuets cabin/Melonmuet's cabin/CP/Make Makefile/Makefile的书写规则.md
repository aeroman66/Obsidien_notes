# 语法
## 基本规则
Target(目标：all) : prerequisites(依赖文件)
	command(命令)
	... 

targets：目标文件名，多个文件以空格分开。
prerequisites：其中任意一个修改日期比target新，或者target不存在了，那么依赖关系发生。
command：命令一定以tab键开头；可以有多行命令


tips：
1. Makefile告诉make文件的依赖关系以及如何构成目标文件的命令。
2. make会以UNIX的标准shell，也就是/bin/sh来执行命令

## 通配符
	通配符替代了一系列的文件

### \*
\*.c 表示所有后缀为.c的文件
### ？
### \[...\]
	这三种通配符用法应该是一样的

## 伪目标
	没有定义生成伪目标所需要的依赖文件，并不生成文件。
### Ex.
clean:
	rm \*.o

### 用于默认目标
### Tips
取名不能和文件名重名，否则就失去了伪目标的意义
用特殊标记显性地定义一个伪目标：
	.
	PHONY:clean
	clean:
		rm \*.o

## 多目标
	多个目标同时依赖于同一个文件，且生成命令大体相似

bigout littleout : text.g
	generate text.g -\$(subst output,,\$@) >;$@

# 命令
	以tab键开头，就认为是一个命令。
1. 当最终目标需要被更新时，make就会一条条执行他之后的命令。
2. 如果要上一条的命令应用于下一条，就需要用分号分隔两条命令，而不能把两条命令写在两行上。
3. 命令执行完毕后，make会检测执行命令的返回码。如果命令返回成功，继续执行。如果返回失败，终止执行当前规则。
	1. 我们可以选择忽略命令出错。在命令前面加一个“-”，不管是否出错都认为他成功。

# 变量
	像是宏，代表一个文本字串，在执行时会自动展开在所使用的地方。变量值可以改变
## 变量基础
变量名：尤其注意可以以数字开头
声明：需要给初值。
使用：变量名前加上$符号，最好用（）或{}将他包起来（为了程序稳定性考虑）
Ex.
	objects = program.o foo.o utils.o
	program:$(objects)
		cc -o program $(objects)
		$(objects):defs.h

## 赋值
### 嵌套定义
Ex.
foo = $(bar)
bar = $(ugh)
ugh = Huh?

### :=操作符
	前面变量不能使用后面变量，只能使用前面定义好的变量
Ex.
y := $(x) bar
x = foo

output:
y:bar 
x:foo

### ?=操作符
	如果变量未被定义过，就赋值给变量。定义过了，这条赋值语句不执行。

### +=操作符
	追加变量值
Ex. 
objects = main.o foo1.o
objects += foo2.o

# 函数调用
	函数返回值可以当作变量来用。与变量使用很像，都是用$来标识的。
	$(<function><arguments> )
多个参数之间用","分隔
Ex.
$(subst <\from>,<\to>,<\str>)
$(padsubst <\pattern>,<\replacement>,<\str>)
$(findstring <\find>,<\  in>)
$(filter %.c,%.o,<\str>)

## 循环函数
	text返回的字符串以空格分割
$(foreach <\var>,<\list>,<\text>)
Ex.
	names := a b c d
	files := \$(foreach n,\$(names),$(n).o)
	$(files) : a.o b.o c.o d.o

## 条件判断函数
	跟C中的大致相当，不同的是make支持四个条件判断关键字。
1. ifeq(<\arg1>,<\arg2>)
2. ifneq(<\arg1>,<\arg2>)
3. ifdef<\variable-name>
4.  ifdef<\variable-name>
### if
$(if<\condition><\then-part><\else-part>)
	else-part未被定义，但是condition为假，那么返回空
# 隐式规则
	makefile预先规定好，不用写出来的规则。比如把.c文件编译成.o文件
	隐式规则会使用一些系统变量，通过改变系统变量可以改变运行参数，还可以通过模式规则自定义隐式规则。
	make可以自动推导的
Ex.
编译C程序的隐式规则命令：
$(CC) -c $(CFLAGS) \$(CPPFLAGS)      \$(CC) = gcc;\$(CFLAGS) = -g
=>gcc -c -g \$(CPPFLAGS)

## 变量种类
### 与命令相关
### 与参数相关

### 自动化变量
把中定义的一系列文件自动地逐个取出，直至所有符合模式的文件都取完为止。 
	只应出现在命令当中。

## 模式规则
	可以用模式规则来定义一个隐式规则
### %
定义对文件名的匹配，表示任意长度的非空字符串。
依赖目标中同样可以使用%
Ex.
"%.c":表示所有以.c结尾的文件
“s.%.c”:表示所有以s.开头，.c结尾的文件，文件名长度最小为5

“%.o:%.c ; <\command>”:指出所有.c文件生成相应的.o文件的规则。如果要生成的目标是a.o,b.o,那么%c就是a.c,b.c