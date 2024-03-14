	文本编辑器对于一个程序员来说十分的重要。与一般的形如word的文本编辑器不一样，写程序跟写文章的需求是不一样的。Vim 启发了很多其他的编辑器，具有代表性，而且用的挺广的。这里主要介绍他背后主要的设计哲学。
Vim 本身的 interface 就是一个 programing language，每个键组合都有着一种功能，一旦你掌握了他们的功能，你可以像编程语言一样把这些键组合组合在一起。而这些组合功能大多是在 normal mode 中实现的，所以 normal mode 是 vim 很重要的一个特性（不要以为 normal mode 是一种 没用多余的模式）以下是这种编程语言拥有的四种元素：
- movements
	- h,j,k,l,w
- edits
	- d,c,x,u,y,p
- counts概念
	- 给命令一个数字，然后让 vim 做某件事情做这个数字次：4j 向下移4行
- modifiers
	- 主要讲的是我想怎么和括号等等这些文本以外的东西交互
	- a  around
	- i   inside：可以帮你选中括号内的内容
以上四种操作可以进行组合以实现特定的功能，就像是编程一样（原来是这个意思）
![[vim_demo]]
# A Model Editor
这意味着 vim 很多的操作模式。下面我们介绍 vim 不同的操作模式。
```shell
vim editors.md // 启动！！
```
把手从键盘移到鼠标上是浪费时间的，所以 vim 的操作都可以在键盘上实现。
## Normal Mode
	Navigating between files.Going from files to files.
- 大部分时间拿来阅读代码
- 删东西
- 进行特殊操作后进入其他模式
	home, where you should be most of the time.
## Insert Mode
	Typing in text
	(i)

## Replace Mode
	(R)

## Modes for Selection
### Visual Mode(V)
可以进行normal mode里的移动操作，但每次移动都会把你光标扫过的区域选中。
常用的操作是选中后进行复制黏贴。
#### Visual Line(shift+v)
用于选取整行
#### Visual Block(ctrl+v)
用于按块选取（方块）

## Command Line Mode
	进入之后鼠标会到屏幕最底下，在那里可以输入命令。

	退出vim
```shell
:quit
```
	退出窗口
```shell
:q  //退出当前窗口
:qa  //quit all
```
	保存文件
```shell
:w
```
	寻求帮助
```shell
:help (key)
```
	开新窗口
```shell
:tabnew
```
# 多窗口
与其他的编辑器逻辑不太一样，一个buffer不一定只对应一个窗口。你可以在两个窗口同时打开同一个文件，方便比如说阅读同一个程序的两个不同部分。
```shell
:sep
```

tabs->windows->buffer

# 自定义
	highly programmable, 不仅仅是命令可以相互组合，还有vim的各种参数是可以编辑的。 
vimrc
	跟大部分shell based tool很像，会有一个plain text file去设置这个工具如何运行。