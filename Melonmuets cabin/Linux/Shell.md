	与计算机交互的最基础的方式。用图形界面交互是有局限的，因为你仅仅能与那些设置了按钮的、图案的东西交互。
执行一个可执行程序
eg: date

执行一个带参数的可执行程序
eg: echo hello
	注意参数之间使用空格分割的“my photo”是两个参数

电脑如何知道如何执行你输入的命令：
电脑有很多的"build-in programs“ 全都保存在你的文件系统里，shell有定位每个program的能力，靠”环境变量“实现。

环境变量：
不必在每次启动shell时都设置一遍。   
eg: $PATH  所有shell用来搜索程序的路径。
	pwd:present working directory
	which echo:打印echo的path
	cd /home:change directory 
	.:current dir
	..:parent dir
		./home
		../home
		../../../../../../../:all the way back to the ...
	relative directory\absolute directory
	ls:list all the files in the current directory
		ls ..
	~ :home directory
	cd -:to the dir you were previously in. 
	mv:move a file or rename 
	cp:copy
	rm:remove a file.
		不是一个recursive的命令，所以不能一下子rm一个dir，是一个防呆机制，防止你一下子把自己的一大文件删掉了。 
	mkdir: 创造一个目录
	man:manue the page
		让一个页面看上去更美观？ 
	cat : prints the contents of a file.
	
windows会分很多个盘 C: D:
linux跟mac则全用一个空间

flags and options:
	 starts with - 
-help 
	ls --help:full command
-l
	ls -l:会给出很多额外信息，除了打印目录之外
		给出每个文件的各种权限 
			read directory
			write directory
			write file 
				要访问一个文件就必须有这个文件所在的每一级目录的权限 

	shell真正的实力是帮你chain multiple programs together, interact with files have files operates in between programs.

Streams:
	每个程序默认有一个input stream 和一个output stream 
在shell中默认的：
input：keyboard
output:shell terminal
	shell有能力去重新编制这些streams

< file:
rewire the input of this program to be the contents of this file.
\> file:
rewire the output of this program  into this file
	echo hello > hello.txt
		输入是echo的键盘输入，echo的输出则进入了hello.txt
	cat <hello.txt > hello2.txt

\>> file:
append then just overwrite. 

	以上也只是直接与文件进行交互的方式，相当的直接
	以下的一些操作符才是真真有趣的地方
Pipe char
	不止可用于文件，还可用于图片信息等
 | 
 take the output of the program to the left and make it the input of the program to the right.
	 ls -l | tail -n1:只输入最后一行
		 | is what wires them together.

# Root user
	在lunix和macOS上，被允许在系统上做任何事情。Super User
一般情况下你不会以Root user来访问Root user。因为假如你不小心运行了什么不正确的程序，你的电脑可能会崩溃，这是一种对你电脑的保护。

sudo:
	super user do.
	You the following things as a super user.

cd /sys
	to enter a whole new world
	里面存的都是你电脑的各种参数。
	Kernel
sudo su:
	以root user执行

sudo echo 500 > brightness
echo 500 > sudo tee brightness
	以上两句是不一样的，以su身份运行的命令是不一样的