	Unified Robot Description Format
是一种统一机器人描述格式，采用的是XML语法。
	个人理解，我们用例如 SW 建模出来的机器人会比较花里胡哨，URDF 则将一些模型细节与关节特征剥离开来，将机器人简化为一个个连杆和关节，每个连杆再关联一个STL文件，以便你未来回复这个机器人模型。

# 标签
只能有一个根标签 \<robot\>，还有常用标签\<link\>\<joint\>，一个完整的机器人是由一系列joint、link组成的。

```XML
<robot>
	<link>
		...
	</link>
	<link>
	...
	</link>
	<joint>
	...
	</joint>
</robot>
```
## \<link\>
展示一些常用的属性和根标签。
```XML
<robot name="linkage">
	<link name="root link">
		<inertial>
		...
		</inertial>
		<visual>
			<geometry>
			...
			</geometry>
			<materail>
			...
			</material>
		</visual>
	</link>
	...
</robot>
```
## \< joint \>
link是通过一定的层次一个个联系在一起的，joint通过 parent-child 将上下两个 links 连接在一起。
```XML
<robot name="linkage">
	<joint name="joint A" ...>
		<parent link="link A" />
		<child link="link B" />
	</joint>
	<joint name="joint A" ...>
		<parent link="link A" />
		<child link="link C" />
	</joint>
</robot>
```
	这里的子标签是 parent child,他们各自有一个属性为 link

## Tips
- 一个 child 只能有一个 parent
- 只有 root link 可以有多个分支
- 一个模型只能有一个 root link
