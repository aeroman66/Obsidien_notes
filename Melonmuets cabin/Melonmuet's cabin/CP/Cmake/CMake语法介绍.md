	变量好像只能用{}来包，否则就不对，很特别
# PROJECT 关键字
## 功能
1. 用来指定工程名字
2. 指定支持的语言（默认支持所有语言）
	PROJECT（HELLO C CXX）
3. 隐式的定义了两个CMake变量
	1. <\projectname>_BINARY_DIR      HELLO_BINARY_DIR
	2. <\projectname>_SOURCE_DIR

# SET 关键词
1. 用来显性地指定变量
	SET(SRC_LIST main.c foo1.c)   (之间用空格进行分割)

# MESSAGE 关键词
	STATUS好像必须大写，否则结果也是不对的
1. 向终端输出用户自定义的信息
	1. SEND_ERROR:产生错误，生成过程被跳过
	2. STATUS：输出前缀为--的消息
	3. FATAL_ERROR:立即终止所有cmake过程

# ADD_EXECUTABLE 关键词
1. 生成可执行文件
	ADD_EXECUTABLE(hello ${SRC_LIST})
		可执行文件名：hello
		源文件读取变量：SRC_LIST

# ADD_SUBDIRECTORY 关键字
1. 用于向当前工程添加存放源文件的子目录（有待探索）
	ADD_SUBDIRECTORY(src bin)  将src子目录加入工程并指定编译输出路径为bin目录



# 基本规则
1. 变量读取方式：${}
2. 指令与参数：指令（参数1 参数2 ...）参数间用空格或分号分开，用括号括起
3. 指令大小写无关，参数与变量大小写相关（建议全部使用大写指令）
## Tips:
1. 工程名和可执行文件名之间没有关系（尽管一般他们看上去非常的像）
2. 文件名可选择是否用双引号框起来（如果文件名中有空格则必须框起来）
3. ADD_EXECUTABLE中参数后缀可以不加（推荐还是加上，会发生混淆的情况）