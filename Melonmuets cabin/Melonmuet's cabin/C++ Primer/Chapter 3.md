# 字符串、向量和数组
	先介绍一些迭代器的相关知识
## 迭代器 Iterator
	是比下标运算符更加通用的操作，是对对象的间接访问。
### 使用迭代器
- 获取迭代器
	- .begin(),.end(),.cbegin(),.cend()
	- 善用auto关键词，因为我们不在意迭代器的准确类型
- 迭代器运算符
	- \*
	- ->
	- ++,--
	- +=,-=
	- \=\=,!=
### 算法
- 二分搜索
## String
	可变长的字符序列，定义在命名空间std中。
	#include<string>
	using std::string
### 初始化方式
	对于string来说，直接初始化和拷贝初始化存在差别，并且拷贝初始化有时不存在任何补偿优势。
- string s1
- string s2(s1)
- string s2 = s1
- string s3("value")
- string s3 = "value"
- string s4(n,'c')

### 操作
#### 基本操作
- os << s,is >> s
	- 读入string对象时，会忽略开头所有空白，直至读到下一个空白为止。
- getline(is,s)
	- 可以保留一些空白符，读到换行符为止。
- s.empty()
- s.size()
- s[n]
- s1+s2
	- 字符串字面值与string是不同类型，在做相加操作时需要注意。
- s1 = s2
- s1 == s2, s1 != s2
- <, <=, >=, >

#### 范围for语句
	for(declaration:expression)
		statement

## vector
	是一个对象的集合，其中所有对象的类型相同。也被称为容器。
	#include <vector>
	using std::vector;
### 初始化方式
	事实上，vector的模板控制着定义和初始化向量的方式，以下先展现一点通用方法。
- vector<\T> v1;
	- 默认初始化，不含任何元素
- vector<\T> v2(v1)；vector<\T> v2 = v1;
	- v2中的元素是v1的副本
- vector<\T> v3(n,val)
- vector<\T> v4(n)
	- 包含了n个执行了值初始化的对象
	- 值初始化的值由vector中元素类型决定。
- 列表初始化{  }
	- 如果提供的是初始元素值列表，那么只能使用列表初始化。

### 操作
- .empty();.size()
- .push_back(t)
	- 把一个值压到vector对象的尾端
- v[n]
	- 返回下表为n的元素的引用。
- v1 = {val1,val2,...}
	- 用列表中元素的拷贝去替换v1中元素
- \=\=;!=
- <, <=, >=, >
tip:
只能对已存在的元素实行下标操作。换言之，不能用下标向容器中添加元素。

## 数组  array
	数组与vector在性能和灵活性的权衡上有所不同，数组的大小固定不变，在某些使用场景下有着更好的性能。
### 定义
	基本内置类型+数组名+维度
- 维度数必须是一个常量表达式。
- 必须指定数组类型，不能用auto来推断。
- 不存在引用的数组。
### 初始化
列表初始化。
	采用列表初始化可以不指定数组的维度。
不允许拷贝与赋值。

### 数组和指针
	string \*p = nums;
	上面这句等价于：p = &nums[0]
新标准还引入了begin与end函数
	int ia = {1,2,3,4,5,6,7,8,9};
	int \*beg = begin(ia);
	int \*end = end(ia);

### 多维数组
To be continued.

























































































































































































































