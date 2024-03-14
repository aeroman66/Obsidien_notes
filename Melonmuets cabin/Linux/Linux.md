---
annotation-target: Linux_Tutor.pdf
---


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":115588,"end":115593},{"type":"TextQuoteSelector","exact":"目录树架构","prefix":"形态来呈现的，所以啰，整个 Linux 系统最重要的地方就是在于","suffix":"。  所谓的目录树架构(directory tree)就是以根目"}]}],"created":"2023-12-01T06:35:52.693Z","updated":"2023-12-01T06:35:52.693Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%形态来呈现的，所以啰，整个 Linux 系统最重要的地方就是在于%%HIGHLIGHT%% ==目录树架构== %%POSTFIX%%。  所谓的目录树架构(directory tree)就是以根目*
>%%LINK%%[[#^2844esuik2s|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#文件, #目录树
^2844esuik2s


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":115693,"end":115709},{"type":"TextQuoteSelector","exact":"根目录的表示方法为一条斜线『/』","prefix":"架构最重要的就是那个根目录(root directory)，这个","suffix":"，  所有的文件都与目录树有关。目录树的呈现方式如下图所示："}]}],"created":"2023-12-01T06:36:12.917Z","updated":"2023-12-01T06:36:12.917Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%架构最重要的就是那个根目录(root directory)，这个%%HIGHLIGHT%% ==根目录的表示方法为一条斜线『/』== %%POSTFIX%%，  所有的文件都与目录树有关。目录树的呈现方式如下图所示：*
>%%LINK%%[[#^nf8d4tkahf8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#文件, #目录树
^nf8d4tkahf8


>%%
>```annotation-json
>{"text":"将一个树状结构映射到磁盘的圆盘形状的空间上","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":115973,"end":115990},{"type":"TextQuoteSelector","exact":"如何结合目录树的架构与磁盘内的数据","prefix":"是我们的文件数据其实是放置在磁盘分区槽当中的，  现在的问题是『","suffix":"』呢？  这个时候就牵扯到『挂载(mount)』的问题啦！ "}]}],"created":"2023-12-01T06:37:58.605Z","updated":"2023-12-01T06:37:58.605Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%是我们的文件数据其实是放置在磁盘分区槽当中的，  现在的问题是『%%HIGHLIGHT%% ==如何结合目录树的架构与磁盘内的数据== %%POSTFIX%%』呢？  这个时候就牵扯到『挂载(mount)』的问题啦！ *
>%%LINK%%[[#^peztp4cucw|show annotation]]
>%%COMMENT%%
>将一个树状结构映射到磁盘的圆盘形状的空间上
>%%TAGS%%
>#硬盘, #目录树, #挂载
^peztp4cucw


>%%
>```annotation-json
>{"text":"注意这里的表述，我们是将一块空间挂载到一个目录。将这个目录作为这块空间的入口，可以把它想象成一个转送门。在一块已经划好的空间内还可以设置新的传送门。","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":116047,"end":116097},{"type":"TextQuoteSelector","exact":"利用一个目录当成进入点，将磁盘分区槽的数据放置在该目录下；  也就是说，进入该目录就可以读取该分区槽","prefix":"问题啦！  文件系统与目录树的关系(挂载) 所谓的『挂载』就是","suffix":"的意思。这个动作我们称为『挂载』，那个进入点的目录我们称为『挂载"}]}],"created":"2023-12-01T06:38:29.538Z","updated":"2023-12-01T06:38:29.538Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%问题啦！  文件系统与目录树的关系(挂载) 所谓的『挂载』就是%%HIGHLIGHT%% ==利用一个目录当成进入点，将磁盘分区槽的数据放置在该目录下；  也就是说，进入该目录就可以读取该分区槽== %%POSTFIX%%的意思。这个动作我们称为『挂载』，那个进入点的目录我们称为『挂载*
>%%LINK%%[[#^atvws5z9yf|show annotation]]
>%%COMMENT%%
>注意这里的表述，我们是将一块空间挂载到一个目录。将这个目录作为这块空间的入口，可以把它想象成一个转送门。在一块已经划好的空间内还可以设置新的传送门。
>%%TAGS%%
>#挂载
^atvws5z9yf


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":163831,"end":163850},{"type":"TextQuoteSelector","exact":"不论空几格  shell  都视为一格","prefix":"； 5. 指令,  选项,  参数等这几个咚咚中间以空格来区分，","suffix":"。所以空格是很重要的特殊字符！； 6. 按下[Enter]按键后"}]}],"created":"2023-12-01T06:51:57.149Z","updated":"2023-12-01T06:51:57.149Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%； 5. 指令,  选项,  参数等这几个咚咚中间以空格来区分，%%HIGHLIGHT%% ==不论空几格  shell  都视为一格== %%POSTFIX%%。所以空格是很重要的特殊字符！； 6. 按下[Enter]按键后*
>%%LINK%%[[#^53lkab8n3xu|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#shell命令
^53lkab8n3xu


>%%
>```annotation-json
>{"text":"反斜杠后面不要接空格！！","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":163930,"end":163952},{"type":"TextQuoteSelector","exact":"反斜杠  (\\)  来跳脱[Enter]符号","prefix":"]按键代表着一行指令的开始启动。 7. 指令太长的时候，可以使用","suffix":"，使指令连续到下一行。注意！反斜杠后就立刻接特殊字符，才能跳脱！"}]}],"created":"2023-12-01T06:52:10.379Z","updated":"2023-12-01T06:52:10.379Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%]按键代表着一行指令的开始启动。 7. 指令太长的时候，可以使用%%HIGHLIGHT%% ==反斜杠  (\)  来跳脱[Enter]符号== %%POSTFIX%%，使指令连续到下一行。注意！反斜杠后就立刻接特殊字符，才能跳脱！*
>%%LINK%%[[#^3t7aqfl3f2l|show annotation]]
>%%COMMENT%%
>反斜杠后面不要接空格！！
>%%TAGS%%
>#shell命令
^3t7aqfl3f2l


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":169769,"end":169785},{"type":"TextQuoteSelector","exact":"直接显示结果然后回到命令提示字符","prefix":"令列模式里面下达指令时，会有两种主要的情况：  一种是该指令会","suffix":"等待下一个指令的输入；  一种是进入到该指令的环境，直到结束该"}]}],"created":"2023-12-01T06:56:05.932Z","updated":"2023-12-01T06:56:05.932Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%令列模式里面下达指令时，会有两种主要的情况：  一种是该指令会%%HIGHLIGHT%% ==直接显示结果然后回到命令提示字符== %%POSTFIX%%等待下一个指令的输入；  一种是进入到该指令的环境，直到结束该*
>%%LINK%%[[#^02r97aqqayhd|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#shell命令
^02r97aqqayhd


>%%
>```annotation-json
>{"text":"听上去好高大上，就是大致存在两种类型的指令","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":169802,"end":169811},{"type":"TextQuoteSelector","exact":"进入到该指令的环境","prefix":"接显示结果然后回到命令提示字符等待下一个指令的输入；  一种是","suffix":"，直到结束该指令才回到命令提示字符的环境。 我们以一个简单的图示"}]}],"created":"2023-12-01T06:56:09.266Z","updated":"2023-12-01T06:56:09.266Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%接显示结果然后回到命令提示字符等待下一个指令的输入；  一种是%%HIGHLIGHT%% ==进入到该指令的环境== %%POSTFIX%%，直到结束该指令才回到命令提示字符的环境。 我们以一个简单的图示*
>%%LINK%%[[#^h7ad8ei9k6e|show annotation]]
>%%COMMENT%%
>听上去好高大上，就是大致存在两种类型的指令
>%%TAGS%%
>#shell命令
^h7ad8ei9k6e


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":171132,"end":171193},{"type":"TextQuoteSelector","exact":"ommand(第一个输入的数据)后面时，他就代表着  『命令补全』，如果是接在第二个字以后的，就会变成『文件补齐』的功能了","prefix":"注意看上面两个例子喔，  我们按[tab]按键的地方如果是在 c","suffix":"！但是在某些特殊的指令底下，文件补齐的功能可能会变成『参数/选项"}]}],"created":"2023-12-01T06:58:15.861Z","updated":"2023-12-01T06:58:15.861Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%注意看上面两个例子喔，  我们按[tab]按键的地方如果是在 c%%HIGHLIGHT%% ==ommand(第一个输入的数据)后面时，他就代表着  『命令补全』，如果是接在第二个字以后的，就会变成『文件补齐』的功能了== %%POSTFIX%%！但是在某些特殊的指令底下，文件补齐的功能可能会变成『参数/选项*
>%%LINK%%[[#^k99hkgf6whc|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#shell命令
^k99hkgf6whc


>%%
>```annotation-json
>{"text":"离开命令行？键盘输入结束是什么意思？","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":172478,"end":172484},{"type":"TextQuoteSelector","exact":"离开文字接口","prefix":"！  另外，他也可以用来取代 exit 的输入呢！例如你想要直接","suffix":"，可以直接按下[Ctrl]-d 就能够直接离开了(相当于输入 e"}]}],"created":"2023-12-01T06:59:25.444Z","updated":"2023-12-01T06:59:25.444Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%！  另外，他也可以用来取代 exit 的输入呢！例如你想要直接%%HIGHLIGHT%% ==离开文字接口== %%POSTFIX%%，可以直接按下[Ctrl]-d 就能够直接离开了(相当于输入 e*
>%%LINK%%[[#^ife7vs6gsi|show annotation]]
>%%COMMENT%%
>离开命令行？键盘输入结束是什么意思？
>%%TAGS%%
>#shell命令
^ife7vs6gsi


>%%
>```annotation-json
>{"created":"2023-12-01T08:06:37.214Z","text":"向硬盘写入数据的命令，在执行关机命令时也会自动调用","updated":"2023-12-01T08:06:37.214Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":193863,"end":193906},{"type":"TextQuoteSelector","exact":" shutdown/reboot/halt  等等指令均已经在关机前进行了  sync","prefix":"关机或重新启动之前，  很重要喔！最好多执行几次！ 虽然目前的 ","suffix":"  这个工具的呼叫，不过，多做几次总是比较放心点～呵呵～ [dm"}]}]}
>```
>%%
>*%%PREFIX%%关机或重新启动之前，  很重要喔！最好多执行几次！ 虽然目前的%%HIGHLIGHT%% ==shutdown/reboot/halt  等等指令均已经在关机前进行了  sync== %%POSTFIX%%这个工具的呼叫，不过，多做几次总是比较放心点～呵呵～ [dm*
>%%LINK%%[[#^xwpduieholf|show annotation]]
>%%COMMENT%%
>向硬盘写入数据的命令，在执行关机命令时也会自动调用
>%%TAGS%%
>
^xwpduieholf


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":201729,"end":201735},{"type":"TextQuoteSelector","exact":"文件的拥有者","prefix":"。  不过，每个文件都有相当多的属性与权限，其中最重要的可能就是","suffix":"的概念了。  所以，在开始文件相关信息的介绍前，鸟哥先就简单的("}]}],"created":"2023-12-01T08:09:22.546Z","updated":"2023-12-01T08:09:22.546Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%。  不过，每个文件都有相当多的属性与权限，其中最重要的可能就是%%HIGHLIGHT%% ==文件的拥有者== %%POSTFIX%%的概念了。  所以，在开始文件相关信息的介绍前，鸟哥先就简单的(*
>%%LINK%%[[#^gdz21a65ws|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#文件, #权限
^gdz21a65ws


>%%
>```annotation-json
>{"text":"多用户多任务就是可以在系统上建立多个用户，而多个用户可以在同一时间内登录同一个系统执行各自不同的任务，而互不影响\n有没有更加具体一点的例子呢","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":201934,"end":201942},{"type":"TextQuoteSelector","exact":"多人多任务的系统","prefix":"健全而好用的一个安全防护呢！怎么说呢？  由于 Linux 是个","suffix":"，因此可能常常会有多人同时使用这部主机来进行工作的情况发生，"}]}],"created":"2023-12-01T08:10:30.864Z","updated":"2023-12-01T08:10:30.864Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%健全而好用的一个安全防护呢！怎么说呢？  由于 Linux 是个%%HIGHLIGHT%% ==多人多任务的系统== %%POSTFIX%%，因此可能常常会有多人同时使用这部主机来进行工作的情况发生，*
>%%LINK%%[[#^op3lfjf1qlk|show annotation]]
>%%COMMENT%%
>多用户多任务就是可以在系统上建立多个用户，而多个用户可以在同一时间内登录同一个系统执行各自不同的任务，而互不影响
>有没有更加具体一点的例子呢
>%%TAGS%%
>#linux
^op3lfjf1qlk


>%%
>```annotation-json
>{"text":"一个群组就是多个用户的集合，这些用户都是登陆在同一个系统上的。一个用户也可以归属于不同的群组。","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":202743,"end":202759},{"type":"TextQuoteSelector","exact":"每个账号都可以有多个群组的支持呢","prefix":"rojecta 与 projectb 这两个群组！』，也就是说：","suffix":"！  这样说或许你还不容易理解这个使用者与群组的关系吧？没关系，"}]}],"created":"2023-12-01T08:13:19.972Z","updated":"2023-12-01T08:13:19.972Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%rojecta 与 projectb 这两个群组！』，也就是说：%%HIGHLIGHT%% ==每个账号都可以有多个群组的支持呢== %%POSTFIX%%！  这样说或许你还不容易理解这个使用者与群组的关系吧？没关系，*
>%%LINK%%[[#^yvkm96m0wo|show annotation]]
>%%COMMENT%%
>一个群组就是多个用户的集合，这些用户都是登陆在同一个系统上的。一个用户也可以归属于不同的群组。
>%%TAGS%%
>#文件, #权限
^yvkm96m0wo


>%%
>```annotation-json
>{"text":"确实很直观，客厅就是组内所有人可以修改的公共文件；自己的房间则是只有文件拥有者才能看到的文件","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":202904,"end":202923},{"type":"TextQuoteSelector","exact":"都有自己的房间，并且共同拥有一个客厅喔","prefix":"大毛家有三个人，分别是王大毛、王二毛与王三毛』，  而且这三个人","suffix":"！ o 使用者的意义：由于王家三人各自拥有自己的房间，所以，"}]}],"created":"2023-12-01T08:14:34.076Z","updated":"2023-12-01T08:14:34.076Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%大毛家有三个人，分别是王大毛、王二毛与王三毛』，  而且这三个人%%HIGHLIGHT%% ==都有自己的房间，并且共同拥有一个客厅喔== %%POSTFIX%%！ o 使用者的意义：由于王家三人各自拥有自己的房间，所以，*
>%%LINK%%[[#^ea5llrt2rei|show annotation]]
>%%COMMENT%%
>确实很直观，客厅就是组内所有人可以修改的公共文件；自己的房间则是只有文件拥有者才能看到的文件
>%%TAGS%%
>#文件, #权限
^ea5llrt2rei


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":203806,"end":203820},{"type":"TextQuoteSelector","exact":"root 可是『万能的天神』","prefix":"x 系统中的身份代号是『  root  』啦！所以要小心喔！那个","suffix":"喔！  无论如何，『使用者身份』，与该使用者所支持的『群组』概念"}]}],"created":"2023-12-01T08:18:32.358Z","updated":"2023-12-01T08:18:32.358Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%x 系统中的身份代号是『  root  』啦！所以要小心喔！那个%%HIGHLIGHT%% ==root 可是『万能的天神』== %%POSTFIX%%喔！  无论如何，『使用者身份』，与该使用者所支持的『群组』概念*
>%%LINK%%[[#^wjg4t334mmj|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#文件, #权限
^wjg4t334mmj


>%%
>```annotation-json
>{"text":"除了拥有者，拥有者所在群组内的成员以外的所有用户，都是others。\n是不是可以设置权限，不能被群组内成员访问，而可以被others访问？","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":203488,"end":203498},{"type":"TextQuoteSelector","exact":"其他人，Others","prefix":"小猪就可以透过三毛进入王家啦！呵呵！没错！那个张小猪就是所谓的『","suffix":"』啰！  因此，我们就可以知道啦，在 Linux 里面，任何一个"}]}],"created":"2023-12-01T08:18:52.452Z","updated":"2023-12-01T08:18:52.452Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%小猪就可以透过三毛进入王家啦！呵呵！没错！那个张小猪就是所谓的『%%HIGHLIGHT%% ==其他人，Others== %%POSTFIX%%』啰！  因此，我们就可以知道啦，在 Linux 里面，任何一个*
>%%LINK%%[[#^v9wc8ihchbp|show annotation]]
>%%COMMENT%%
>除了拥有者，拥有者所在群组内的成员以外的所有用户，都是others。
>是不是可以设置权限，不能被群组内成员访问，而可以被others访问？
>%%TAGS%%
>#文件, #权限
^v9wc8ihchbp


>%%
>```annotation-json
>{"text":"记录下这个可能出现的错误","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":204925,"end":204940},{"type":"TextQuoteSelector","exact":"Permission deny","prefix":"么你将老是听不懂别人在讲什么呢！尤其是当你在你的屏幕前面出现了『","suffix":"』的时候，不要担心，『肯定是权限设定错误』啦！呵呵！好了，闲话不"}]}],"created":"2023-12-01T08:23:16.945Z","updated":"2023-12-01T08:23:16.945Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%么你将老是听不懂别人在讲什么呢！尤其是当你在你的屏幕前面出现了『%%HIGHLIGHT%% ==Permission deny== %%POSTFIX%%』的时候，不要担心，『肯定是权限设定错误』啦！呵呵！好了，闲话不*
>%%LINK%%[[#^ad7nbe03l9w|show annotation]]
>%%COMMENT%%
>记录下这个可能出现的错误
>%%TAGS%%
>#权限
^ad7nbe03l9w


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":206811,"end":206863},{"type":"TextQuoteSelector","exact":"[ r ]代表可读(read)、[ w ]代表可写(write)、[ x ]代表可执行(execute)","prefix":"符中，以三个为一组，且均为『rwx』  的三个参数的组合。其中，","suffix":"。  要注意的是，这三个权限的位置不会改变，如果没有权限，就会出"}]}],"created":"2023-12-01T08:28:11.368Z","updated":"2023-12-01T08:28:11.368Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%符中，以三个为一组，且均为『rwx』  的三个参数的组合。其中，%%HIGHLIGHT%% ==[ r ]代表可读(read)、[ w ]代表可写(write)、[ x ]代表可执行(execute)== %%POSTFIX%%。  要注意的是，这三个权限的位置不会改变，如果没有权限，就会出*
>%%LINK%%[[#^nlgjmjd76p|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#权限
^nlgjmjd76p


>%%
>```annotation-json
>{"text":"这里倒是体现了linux中的所有硬件都是以文件形式存在的这一思想\n目录也是一种文件？","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":206558,"end":206568},{"type":"TextQuoteSelector","exact":"目录、文件或链接文件","prefix":".2.2、文件的类型与权限之内容  第一个字符代表这个文件是『","suffix":"等等』： o 当为[ d ]则是目录，例如上表档名为『.conf"}]}],"created":"2023-12-01T08:29:09.936Z","updated":"2023-12-01T08:29:09.936Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%.2.2、文件的类型与权限之内容  第一个字符代表这个文件是『%%HIGHLIGHT%% ==目录、文件或链接文件== %%POSTFIX%%等等』： o 当为[ d ]则是目录，例如上表档名为『.conf*
>%%LINK%%[[#^9za35kz37um|show annotation]]
>%%COMMENT%%
>这里倒是体现了linux中的所有硬件都是以文件形式存在的这一思想
>目录也是一种文件？
>%%TAGS%%
>#文件
^9za35kz37um


>%%
>```annotation-json
>{"created":"2023-12-01T08:30:10.861Z","text":"所有权限都是针对账号而言的，而前面我们已经将所有的账号分为了三种类型。","updated":"2023-12-01T08:30:10.861Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":207059,"end":207071},{"type":"TextQuoteSelector","exact":"针对某些账号来设计的权限","prefix":"。  Tips 请你特别注意喔！不论是那一组权限，基本上，都是『","suffix":"』喔！以群组来说，他规范的是『加入这个群组的账号具有什么样的权限"}]}]}
>```
>%%
>*%%PREFIX%%。  Tips 请你特别注意喔！不论是那一组权限，基本上，都是『%%HIGHLIGHT%% ==针对某些账号来设计的权限== %%POSTFIX%%』喔！以群组来说，他规范的是『加入这个群组的账号具有什么样的权限*
>%%LINK%%[[#^ieqs8ewzbn9|show annotation]]
>%%COMMENT%%
>所有权限都是针对账号而言的，而前面我们已经将所有的账号分为了三种类型。
>%%TAGS%%
>
^ieqs8ewzbn9


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":206887,"end":206903},{"type":"TextQuoteSelector","exact":"没有权限，就会出现减号[ - ]","prefix":"execute)。  要注意的是，这三个权限的位置不会改变，如果","suffix":"而已。 o 第一组为『文件拥有者可具备的权限』，以『initia"}]}],"created":"2023-12-01T08:31:17.804Z","updated":"2023-12-01T08:31:17.804Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%execute)。  要注意的是，这三个权限的位置不会改变，如果%%HIGHLIGHT%% ==没有权限，就会出现减号[ - ]== %%POSTFIX%%而已。 o 第一组为『文件拥有者可具备的权限』，以『initia*
>%%LINK%%[[#^6549k5aqic3|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#权限
^6549k5aqic3


>%%
>```annotation-json
>{"created":"2023-12-01T08:31:39.209Z","updated":"2023-12-01T08:31:39.209Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":207472,"end":207510},{"type":"TextQuoteSelector","exact":"目录与文件的权限意义并不相同，这是因为目录与文件所记录的数据内容不相同所致。","prefix":"有该权限就会显示字符，没有该权限就变成减号(-)就是了。 另外，","suffix":"  由于目录与文件的权限意义非常的重要，所以鸟哥将他独立到 5."}]}]}
>```
>%%
>*%%PREFIX%%有该权限就会显示字符，没有该权限就变成减号(-)就是了。 另外，%%HIGHLIGHT%% ==目录与文件的权限意义并不相同，这是因为目录与文件所记录的数据内容不相同所致。== %%POSTFIX%%由于目录与文件的权限意义非常的重要，所以鸟哥将他独立到 5.*
>%%LINK%%[[#^1yzogawi81l|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^1yzogawi81l


>%%
>```annotation-json
>{"created":"2023-12-01T08:34:05.467Z","text":"文件怎么所属某个组群啊\n万一文件用户加入了多个组群呢？","updated":"2023-12-01T08:34:05.467Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":207877,"end":207896},{"type":"TextQuoteSelector","exact":"某个文件所属的群组为 projecta","prefix":"ass2, class3均属于 projecta 这个群组，假设","suffix":"，且该文件的权限如图 5.2.2 所示(-rwxrwx---)，"}]}]}
>```
>%%
>*%%PREFIX%%ass2, class3均属于 projecta 这个群组，假设%%HIGHLIGHT%% ==某个文件所属的群组为 projecta== %%POSTFIX%%，且该文件的权限如图 5.2.2 所示(-rwxrwx---)，*
>%%LINK%%[[#^dkc6coazuog|show annotation]]
>%%COMMENT%%
>文件怎么所属某个组群啊
>万一文件用户加入了多个组群呢？
>%%TAGS%%
>
^dkc6coazuog


>%%
>```annotation-json
>{"created":"2023-12-01T08:36:01.958Z","text":"就是文件名吧，好抽象的名字","updated":"2023-12-01T08:36:01.958Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":208768,"end":208770},{"type":"TextQuoteSelector","exact":"档名","prefix":"量成为上述的内容即可。  第七栏为这个文件的档名 这个字段就是","suffix":"了。比较特殊的是：如果档名之前多一个『  .  』，则代表这个文"}]}]}
>```
>%%
>*%%PREFIX%%量成为上述的内容即可。  第七栏为这个文件的档名 这个字段就是%%HIGHLIGHT%% ==档名== %%POSTFIX%%了。比较特殊的是：如果档名之前多一个『  .  』，则代表这个文*
>%%LINK%%[[#^72sk9qpc1fx|show annotation]]
>%%COMMENT%%
>就是文件名吧，好抽象的名字
>%%TAGS%%
>
^72sk9qpc1fx


>%%
>```annotation-json
>{"created":"2023-12-01T08:39:04.410Z","text":"因为我还没体验过多用户的操作，所以对这些还没什么概念。看来linux与我的认知还是有很大的差别的。","updated":"2023-12-01T08:39:04.410Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":209988,"end":209993},{"type":"TextQuoteSelector","exact":"数据安全性","prefix":"，尤其是群组的概念，这样有什么用途呢？  其实，最大的用途是在『","suffix":"』上面的。  系统保护的功能： 举个简单的例子，在你的系统中，"}]}]}
>```
>%%
>*%%PREFIX%%，尤其是群组的概念，这样有什么用途呢？  其实，最大的用途是在『%%HIGHLIGHT%% ==数据安全性== %%POSTFIX%%』上面的。  系统保护的功能： 举个简单的例子，在你的系统中，*
>%%LINK%%[[#^oo99n5djpo|show annotation]]
>%%COMMENT%%
>因为我还没体验过多用户的操作，所以对这些还没什么概念。看来linux与我的认知还是有很大的差别的。
>%%TAGS%%
>
^oo99n5djpo


>%%
>```annotation-json
>{"created":"2023-12-01T08:39:29.730Z","text":"天神的存在，他是不属于others之列的","updated":"2023-12-01T08:39:29.730Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":210195,"end":210215},{"type":"TextQuoteSelector","exact":"root 基本上是不受系统的权限所限制的","prefix":"为[ ---------- ]啰！咦！所有人都不能使用？没关系，","suffix":"，  所以无论文件权限为何，预设 root 都可以存取喔！  "}]}]}
>```
>%%
>*%%PREFIX%%为[ ---------- ]啰！咦！所有人都不能使用？没关系，%%HIGHLIGHT%% ==root 基本上是不受系统的权限所限制的== %%POSTFIX%%，  所以无论文件权限为何，预设 root 都可以存取喔！ *
>%%LINK%%[[#^g1ejrhoeqhg|show annotation]]
>%%COMMENT%%
>天神的存在，他是不属于others之列的
>%%TAGS%%
>
^g1ejrhoeqhg


>%%
>```annotation-json
>{"created":"2023-12-01T08:43:35.067Z","text":"必须是登记过的组，不能是非法组？？\n继续去了解一下","updated":"2023-12-01T08:43:35.067Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":211113,"end":211139},{"type":"TextQuoteSelector","exact":"被改变的组名必须要在/etc/group 文件内存在","prefix":"oup 的缩写嘛！这样就很好记了吧！  ^_^。不过，请记得，要","suffix":"才行，否则就会显示错误！ 假设你已经是 root 的身份了，那么"}]}]}
>```
>%%
>*%%PREFIX%%oup 的缩写嘛！这样就很好记了吧！  ^_^。不过，请记得，要%%HIGHLIGHT%% ==被改变的组名必须要在/etc/group 文件内存在== %%POSTFIX%%才行，否则就会显示错误！ 假设你已经是 root 的身份了，那么*
>%%LINK%%[[#^81kkjqg934|show annotation]]
>%%COMMENT%%
>必须是登记过的组，不能是非法组？？
>继续去了解一下
>%%TAGS%%
>
^81kkjqg934


>%%
>```annotation-json
>{"created":"2023-12-01T08:54:07.945Z","text":"[-R]","updated":"2023-12-01T08:54:07.945Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":211462,"end":211477},{"type":"TextQuoteSelector","exact":"变更某一目录内所有的文件之情况","prefix":"录下的所有文件、目录      都更新成为这个群组之意。常常用在","suffix":"。 范例： [root@study ~]# chgrp user"}]}]}
>```
>%%
>*%%PREFIX%%录下的所有文件、目录      都更新成为这个群组之意。常常用在%%HIGHLIGHT%% ==变更某一目录内所有的文件之情况== %%POSTFIX%%。 范例： [root@study ~]# chgrp user*
>%%LINK%%[[#^u07w5nmpuaj|show annotation]]
>%%COMMENT%%
>[-R]
>%%TAGS%%
>
^u07w5nmpuaj


>%%
>```annotation-json
>{"created":"2023-12-01T08:55:33.064Z","updated":"2023-12-01T08:55:33.064Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":211941,"end":211985},{"type":"TextQuoteSelector","exact":"用户必须是已经存在系统中的账号，也就是在/etc/passwd 这个文件中有纪录的用户名","prefix":"BINGO！那就是 chown 这个指令的用途，要注意的是，  ","suffix":"称才能改变。 chown 的用途还满多的，他还可以顺便直接修改群"}]}]}
>```
>%%
>*%%PREFIX%%BINGO！那就是 chown 这个指令的用途，要注意的是，%%HIGHLIGHT%% ==用户必须是已经存在系统中的账号，也就是在/etc/passwd 这个文件中有纪录的用户名== %%POSTFIX%%称才能改变。 chown 的用途还满多的，他还可以顺便直接修改群*
>%%LINK%%[[#^kcigrv4a5h|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^kcigrv4a5h


>%%
>```annotation-json
>{"created":"2023-12-01T08:56:47.540Z","updated":"2023-12-01T08:56:47.540Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":212010,"end":212021},{"type":"TextQuoteSelector","exact":"顺便直接修改群组的名称","prefix":"有纪录的用户名称才能改变。 chown 的用途还满多的，他还可以","suffix":"呢！此外，如果要连目录下的所有次目录或文件同时更改文件拥有者的话"}]}]}
>```
>%%
>*%%PREFIX%%有纪录的用户名称才能改变。 chown 的用途还满多的，他还可以%%HIGHLIGHT%% ==顺便直接修改群组的名称== %%POSTFIX%%呢！此外，如果要连目录下的所有次目录或文件同时更改文件拥有者的话*
>%%LINK%%[[#^fximc7hvz96|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^fximc7hvz96


>%%
>```annotation-json
>{"created":"2023-12-01T09:00:39.876Z","text":"根据一些数学原理，加出来的数字跟你的权限配置是双射关系","updated":"2023-12-01T09:00:39.876Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":213666,"end":213670},{"type":"TextQuoteSelector","exact":"需要累加","prefix":"r/group/others)各自的三个权限(r/w/x)分数是","suffix":"的，例如当权限为：  [-rwxrwx---]  分数则是： o"}]}]}
>```
>%%
>*%%PREFIX%%r/group/others)各自的三个权限(r/w/x)分数是%%HIGHLIGHT%% ==需要累加== %%POSTFIX%%的，例如当权限为：  [-rwxrwx---]  分数则是： o*
>%%LINK%%[[#^wpw3mi6szn|show annotation]]
>%%COMMENT%%
>根据一些数学原理，加出来的数字跟你的权限配置是双射关系
>%%TAGS%%
>
^wpw3mi6szn


>%%
>```annotation-json
>{"created":"2023-12-01T09:07:37.424Z","text":"加了空格数据流的分割就出问题了","updated":"2023-12-01T09:07:37.424Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":215047,"end":215055},{"type":"TextQuoteSelector","exact":"并没有任何空格符","prefix":"c # 注意喔！那个 u=rwx,go=rx 是连在一起的，中间","suffix":"！ [root@study ~]# ls -al .bashrc"}]}]}
>```
>%%
>*%%PREFIX%%c # 注意喔！那个 u=rwx,go=rx 是连在一起的，中间%%HIGHLIGHT%% ==并没有任何空格符== %%POSTFIX%%！ [root@study ~]# ls -al .bashrc*
>%%LINK%%[[#^4c80zd31lp3|show annotation]]
>%%COMMENT%%
>加了空格数据流的分割就出问题了
>%%TAGS%%
>
^4c80zd31lp3


>%%
>```annotation-json
>{"created":"2023-12-01T09:08:31.680Z","text":"这种设计思想跟vim指令的设计还挺像的","updated":"2023-12-01T09:08:31.680Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":215673,"end":215731},{"type":"TextQuoteSelector","exact":"+, -, =  的不同点了吗？对啦！  +  与  –  的状态下，只要是没有指定到的项目，则该权限『不会被变动』","prefix":" 644 .bashrc  # 测试完毕得要改回来喔！ 知道  ","suffix":"， 例如上面的例子中，由于仅以  –  拿掉  x  则其他两个"}]}]}
>```
>%%
>*%%PREFIX%%644 .bashrc  # 测试完毕得要改回来喔！ 知道%%HIGHLIGHT%% ==+, -, =  的不同点了吗？对啦！  +  与  –  的状态下，只要是没有指定到的项目，则该权限『不会被变动』== %%POSTFIX%%， 例如上面的例子中，由于仅以  –  拿掉  x  则其他两个*
>%%LINK%%[[#^taaq70f0qzj|show annotation]]
>%%COMMENT%%
>这种设计思想跟vim指令的设计还挺像的
>%%TAGS%%
>
^taaq70f0qzj


>%%
>```annotation-json
>{"created":"2023-12-01T09:31:22.631Z","updated":"2023-12-01T09:31:22.631Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":216137,"end":216175},{"type":"TextQuoteSelector","exact":"文件是实际含有数据的地方，包括一般文本文件、数据库内容文件、二进制可执行文件","prefix":"不同啊！底下就让鸟哥来说清楚，讲明白！  权限对文件的重要性 ","suffix":"(binary program)等等。  因此，权限对于文件来说"}]}]}
>```
>%%
>*%%PREFIX%%不同啊！底下就让鸟哥来说清楚，讲明白！  权限对文件的重要性%%HIGHLIGHT%% ==文件是实际含有数据的地方，包括一般文本文件、数据库内容文件、二进制可执行文件== %%POSTFIX%%(binary program)等等。  因此，权限对于文件来说*
>%%LINK%%[[#^fm3v437swfu|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^fm3v437swfu


>%%
>```annotation-json
>{"created":"2023-12-01T09:32:06.566Z","text":"意思是，即使是个文本文件，执行起来没有什么意义，但是如果他有可执行权限，那么他也是可执行文件。","updated":"2023-12-01T09:32:06.566Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":216454,"end":216498},{"type":"TextQuoteSelector","exact":"我们的文件是否能被执行，则是藉由是否具有『x』这个权限来决定的！跟档名是没有绝对的关系的","prefix":"xe, .bat, .com  等等，但是在 Linux 底下，","suffix":"！ 至于最后一个 w 这个权限呢？当你对一个文件具有 w 权限时"}]}]}
>```
>%%
>*%%PREFIX%%xe, .bat, .com  等等，但是在 Linux 底下，%%HIGHLIGHT%% ==我们的文件是否能被执行，则是藉由是否具有『x』这个权限来决定的！跟档名是没有绝对的关系的== %%POSTFIX%%！ 至于最后一个 w 这个权限呢？当你对一个文件具有 w 权限时*
>%%LINK%%[[#^pzwdrjrzh4|show annotation]]
>%%COMMENT%%
>意思是，即使是个文本文件，执行起来没有什么意义，但是如果他有可执行权限，那么他也是可执行文件。
>%%TAGS%%
>
^pzwdrjrzh4


>%%
>```annotation-json
>{"created":"2023-12-01T09:33:13.431Z","updated":"2023-12-01T09:33:13.431Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":216557,"end":216619},{"type":"TextQuoteSelector","exact":"但并不具备有删除该文件本身的权限！对于文件的 rwx 来说，  主要都是针对『文件的内容』而言，与文件档名的存在与否没有关系","prefix":"w 权限时，你可以具有写入/编辑/新增/修改文件的内容的权限， ","suffix":"喔！因为文件记录的是实际的数据嘛！  权限对目录的重要性 文件"}]}]}
>```
>%%
>*%%PREFIX%%w 权限时，你可以具有写入/编辑/新增/修改文件的内容的权限，%%HIGHLIGHT%% ==但并不具备有删除该文件本身的权限！对于文件的 rwx 来说，  主要都是针对『文件的内容』而言，与文件档名的存在与否没有关系== %%POSTFIX%%喔！因为文件记录的是实际的数据嘛！  权限对目录的重要性 文件*
>%%LINK%%[[#^f98hhthvn|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^f98hhthvn


>%%
>```annotation-json
>{"created":"2023-12-01T09:34:35.768Z","updated":"2023-12-01T09:34:35.768Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":216676,"end":216704},{"type":"TextQuoteSelector","exact":"目录主要的内容在记录文件名列表，文件名与目录有强烈的关连","prefix":"的重要性 文件是存放实际数据的所在，那么目录主要是储存啥玩意啊？","suffix":"啦！  所以如果是针对目录时，那个  r, w, x  对目录是"}]}]}
>```
>%%
>*%%PREFIX%%的重要性 文件是存放实际数据的所在，那么目录主要是储存啥玩意啊？%%HIGHLIGHT%% ==目录主要的内容在记录文件名列表，文件名与目录有强烈的关连== %%POSTFIX%%啦！  所以如果是针对目录时，那个  r, w, x  对目录是*
>%%LINK%%[[#^1cpodme67vy|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^1cpodme67vy


>%%
>```annotation-json
>{"created":"2023-12-01T09:34:49.419Z","text":"因为两者存储的内容是不一样的，所以权限对他们来说也有不一样的含义。","updated":"2023-12-01T09:34:49.419Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":216078,"end":216097},{"type":"TextQuoteSelector","exact":"文件权限对于一般文件与目录文件有何不同","prefix":"  前两小节也谈到了这些文件权限对于数据安全的重要性。那么，这些","suffix":"呢？  有大大的不同啊！底下就让鸟哥来说清楚，讲明白！  权限"}]}]}
>```
>%%
>*%%PREFIX%%前两小节也谈到了这些文件权限对于数据安全的重要性。那么，这些%%HIGHLIGHT%% ==文件权限对于一般文件与目录文件有何不同== %%POSTFIX%%呢？  有大大的不同啊！底下就让鸟哥来说清楚，讲明白！  权限*
>%%LINK%%[[#^wxnkpqnqsno|show annotation]]
>%%COMMENT%%
>因为两者存储的内容是不一样的，所以权限对他们来说也有不一样的含义。
>%%TAGS%%
>
^wxnkpqnqsno


>%%
>```annotation-json
>{"created":"2023-12-01T09:35:38.528Z","text":"利用这个权限就可以来删除文件啦","updated":"2023-12-01T09:35:38.528Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":217043,"end":217062},{"type":"TextQuoteSelector","exact":"w 权限就与该目录底下的文件名异动有关","prefix":"进行更名； o 搬移该目录内的文件、目录位置。  总之，目录的 ","suffix":"就对了啦！  x (access directory)：  咦"}]}]}
>```
>%%
>*%%PREFIX%%进行更名； o 搬移该目录内的文件、目录位置。  总之，目录的%%HIGHLIGHT%% ==w 权限就与该目录底下的文件名异动有关== %%POSTFIX%%就对了啦！  x (access directory)：  咦*
>%%LINK%%[[#^x3oazwa1toi|show annotation]]
>%%COMMENT%%
>利用这个权限就可以来删除文件啦
>%%TAGS%%
>
^x3oazwa1toi


>%%
>```annotation-json
>{"created":"2023-12-01T09:36:13.276Z","text":"就是能不能进这个目录\n图形化理解就是双击后能不能进去？","updated":"2023-12-01T09:36:13.276Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":217144,"end":217169},{"type":"TextQuoteSelector","exact":" x 代表的是用户能否进入该目录成为工作目录的用途","prefix":"记录文件名而已，总不能拿来执行吧？没错！目录不可以被执行，目录的","suffix":"！  所谓的工作目录(work directory)就是你目前所"}]}]}
>```
>%%
>*%%PREFIX%%记录文件名而已，总不能拿来执行吧？没错！目录不可以被执行，目录的%%HIGHLIGHT%% ==x 代表的是用户能否进入该目录成为工作目录的用途== %%POSTFIX%%！  所谓的工作目录(work directory)就是你目前所*
>%%LINK%%[[#^8nh4gda97pi|show annotation]]
>%%COMMENT%%
>就是能不能进这个目录
>图形化理解就是双击后能不能进去？
>%%TAGS%%
>
^8nh4gda97pi


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":206282,"end":206305},{"type":"TextQuoteSelector","exact":"『-al』则表示列出所有的文件详细的权限与属性","prefix":"是『list』的意思，重点在显示文件的文件名与相关属性。而选项","suffix":"(包含隐藏文件，就是文件名第一个字符为『  .  』的文件)"}]}],"created":"2023-12-03T05:04:25.915Z","updated":"2023-12-03T05:04:25.915Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%是『list』的意思，重点在显示文件的文件名与相关属性。而选项%%HIGHLIGHT%% ==『-al』则表示列出所有的文件详细的权限与属性== %%POSTFIX%%(包含隐藏文件，就是文件名第一个字符为『  .  』的文件)*
>%%LINK%%[[#^d408gshne3l|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#文件, #权限, #shell命令
^d408gshne3l


>%%
>```annotation-json
>{"created":"2023-12-03T05:09:39.764Z","text":"在该目录下执行各种指令，尽管包含了对文件的增删，但是范围大于此","updated":"2023-12-03T05:09:39.764Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":218112,"end":218181},{"type":"TextQuoteSelector","exact":"如果你在某目录下不具有 x 的权限，  那么你就无法切换到该目录下，也就无法执行该目录下的任何指令，即使你具有该目录的 r 或 w 的权限","prefix":" x 权限有关啦！此外，  工作目录对于指令的执行是非常重要的，","suffix":"。 很多朋友在架设网站的时候都会卡在一些权限的设定上，他们开放目"}]}]}
>```
>%%
>*%%PREFIX%%x 权限有关啦！此外，  工作目录对于指令的执行是非常重要的，%%HIGHLIGHT%% ==如果你在某目录下不具有 x 的权限，  那么你就无法切换到该目录下，也就无法执行该目录下的任何指令，即使你具有该目录的 r 或 w 的权限== %%POSTFIX%%。 很多朋友在架设网站的时候都会卡在一些权限的设定上，他们开放目*
>%%LINK%%[[#^vi3yxgb2gf|show annotation]]
>%%COMMENT%%
>在该目录下执行各种指令，尽管包含了对文件的增删，但是范围大于此
>%%TAGS%%
>
^vi3yxgb2gf


>%%
>```annotation-json
>{"created":"2023-12-03T05:11:03.653Z","text":"对上段话的说明","updated":"2023-12-03T05:11:03.653Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":218267,"end":218289},{"type":"TextQuoteSelector","exact":"无法到该目录下读取文件(最多只能看到文件名)","prefix":" 的权限，如上面的范例所示那样，那样的结果就是导致网站服务器软件","suffix":"，  最终用户总是无法正确的查阅到文件的内容(显示权限不足啊！)"}]}]}
>```
>%%
>*%%PREFIX%%的权限，如上面的范例所示那样，那样的结果就是导致网站服务器软件%%HIGHLIGHT%% ==无法到该目录下读取文件(最多只能看到文件名)== %%POSTFIX%%，  最终用户总是无法正确的查阅到文件的内容(显示权限不足啊！)*
>%%LINK%%[[#^oaw06nb3btp|show annotation]]
>%%COMMENT%%
>对上段话的说明
>%%TAGS%%
>
^oaw06nb3btp


>%%
>```annotation-json
>{"created":"2023-12-03T05:15:10.174Z","text":"cd意义","updated":"2023-12-03T05:15:10.174Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":220344,"end":220368},{"type":"TextQuoteSelector","exact":"目录变成工作目录(用  cd  进入该目录之意)","prefix":"录的文件名列表，不过详细的信息却还是读不到的，  同时也不能将该","suffix":"。那如果我们让该目录变成用户的， 那么用户在这个目录底下是否能够"}]}]}
>```
>%%
>*%%PREFIX%%录的文件名列表，不过详细的信息却还是读不到的，  同时也不能将该%%HIGHLIGHT%% ==目录变成工作目录(用  cd  进入该目录之意)== %%POSTFIX%%。那如果我们让该目录变成用户的， 那么用户在这个目录底下是否能够*
>%%LINK%%[[#^bhoj97beqqk|show annotation]]
>%%COMMENT%%
>cd意义
>%%TAGS%%
>
^bhoj97beqqk


>%%
>```annotation-json
>{"created":"2023-12-03T05:17:35.271Z","text":"删除目录需要目录执行权限\n","updated":"2023-12-03T05:17:35.271Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":221493,"end":221504},{"type":"TextQuoteSelector","exact":"具有目录修改的权限即可","prefix":"  file1  文件 wx - - 能够进入  /dir1  ","suffix":"！ 将  file1  复制到  /dir2 x r wx 要能"}]}]}
>```
>%%
>*%%PREFIX%%file1  文件 wx - - 能够进入  /dir1%%HIGHLIGHT%% ==具有目录修改的权限即可== %%POSTFIX%%！ 将  file1  复制到  /dir2 x r wx 要能*
>%%LINK%%[[#^utvqkz780xl|show annotation]]
>%%COMMENT%%
>删除目录需要目录执行权限
>
>%%TAGS%%
>
^utvqkz780xl


>%%
>```annotation-json
>{"created":"2023-12-03T05:18:20.304Z","text":"大多数时候 r 的真正用途","updated":"2023-12-03T05:18:20.304Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":221769,"end":221804},{"type":"TextQuoteSelector","exact":"没有 r  的话，使用  [tab]  时，他就无法自动帮你补齐档名了","prefix":"面很多动作中，你只要具有  x  即可！r  是非必备的！只是，","suffix":"！这样理解乎？ Tips 看了上面这个表格，你应该会觉得很可怕喔"}]}]}
>```
>%%
>*%%PREFIX%%面很多动作中，你只要具有  x  即可！r  是非必备的！只是，%%HIGHLIGHT%% ==没有 r  的话，使用  [tab]  时，他就无法自动帮你补齐档名了== %%POSTFIX%%！这样理解乎？ Tips 看了上面这个表格，你应该会觉得很可怕喔*
>%%LINK%%[[#^6jat2v8pksi|show annotation]]
>%%COMMENT%%
>大多数时候 r 的真正用途
>%%TAGS%%
>
^6jat2v8pksi


>%%
>```annotation-json
>{"created":"2023-12-03T05:19:12.009Z","text":"因为需要将目录变为工作目录，在工作目录下执行读取文件的命令","updated":"2023-12-03T05:19:12.009Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":221895,"end":221904},{"type":"TextQuoteSelector","exact":"rx  这两个权限","prefix":"  x  权限』才行！所以，通常要开放的目录，  至少会具备  ","suffix":"！现在你知道为啥了吧？  5.2.4 Linux 文件种类与扩展"}]}]}
>```
>%%
>*%%PREFIX%%x  权限』才行！所以，通常要开放的目录，  至少会具备%%HIGHLIGHT%% ==rx  这两个权限== %%POSTFIX%%！现在你知道为啥了吧？  5.2.4 Linux 文件种类与扩展*
>%%LINK%%[[#^smhrt1ngl7d|show annotation]]
>%%COMMENT%%
>因为需要将目录变为工作目录，在工作目录下执行读取文件的命令
>%%TAGS%%
>
^smhrt1ngl7d


>%%
>```annotation-json
>{"created":"2023-12-03T05:21:39.040Z","updated":"2023-12-03T05:21:39.040Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":222310,"end":222343},{"type":"TextQuoteSelector","exact":"纯文本档是因为内容为我们人类可以直接读到的数据，例如数字、字母等等","prefix":"CII)：这是 Linux 系统中最多的一种文件类型啰，  称为","suffix":"。  几乎只要我们可以用来做为设定的文件都属于这一种文件类型。 "}]}]}
>```
>%%
>*%%PREFIX%%CII)：这是 Linux 系统中最多的一种文件类型啰，  称为%%HIGHLIGHT%% ==纯文本档是因为内容为我们人类可以直接读到的数据，例如数字、字母等等== %%POSTFIX%%。  几乎只要我们可以用来做为设定的文件都属于这一种文件类型。*
>%%LINK%%[[#^r775cte0yg9|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^r775cte0yg9


>%%
>```annotation-json
>{"created":"2023-12-03T05:22:01.791Z","updated":"2023-12-03T05:22:01.791Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":222544,"end":222549},{"type":"TextQuoteSelector","exact":"可执行文件","prefix":"(binary file)吧？没错～  你的 Linux 当中的","suffix":"(scripts,  文字型批处理文件不算)就是这种格式的啦～ "}]}]}
>```
>%%
>*%%PREFIX%%(binary file)吧？没错～  你的 Linux 当中的%%HIGHLIGHT%% ==可执行文件== %%POSTFIX%%(scripts,  文字型批处理文件不算)就是这种格式的啦～*
>%%LINK%%[[#^m01k80kjhn|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^m01k80kjhn


>%%
>```annotation-json
>{"created":"2023-12-03T05:23:11.114Z","text":"不是简单的将文本文件按特定格式进行排布","updated":"2023-12-03T05:23:11.114Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":222633,"end":222689},{"type":"TextQuoteSelector","exact":"有些程序在运作的过程当中会读取某些特定格式的文件，那些特定格式的文件可以被称为数据文件  (data file)","prefix":"一个binary file。 o 数据格式文件(data)：  ","suffix":"。举例来说，我们的 Linux 在使用者登入时，都会将登录的数据"}]}]}
>```
>%%
>*%%PREFIX%%一个binary file。 o 数据格式文件(data)：%%HIGHLIGHT%% ==有些程序在运作的过程当中会读取某些特定格式的文件，那些特定格式的文件可以被称为数据文件  (data file)== %%POSTFIX%%。举例来说，我们的 Linux 在使用者登入时，都会将登录的数据*
>%%LINK%%[[#^tvrhhvr5tg|show annotation]]
>%%COMMENT%%
>不是简单的将文本文件按特定格式进行排布
>%%TAGS%%
>
^tvrhhvr5tg


>%%
>```annotation-json
>{"created":"2023-12-03T05:25:01.108Z","updated":"2023-12-03T05:25:01.108Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":222907,"end":222911},{"type":"TextQuoteSelector","exact":"快捷方式","prefix":"  连结档(link)： 就是类似 Windows 系统底下的","suffix":"啦！  第一个属性为  [ l ](英文 L 的小写)，例如  "}]}]}
>```
>%%
>*%%PREFIX%% 连结档(link)： 就是类似 Windows 系统底下的%%HIGHLIGHT%% ==快捷方式== %%POSTFIX%%啦！  第一个属性为  [ l ](英文 L 的小写)，例如*
>%%LINK%%[[#^5j3p6qiw3m2|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^5j3p6qiw3m2


>%%
>```annotation-json
>{"created":"2023-12-03T05:26:24.973Z","updated":"2023-12-03T05:26:24.973Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":223003,"end":223007},{"type":"TextQuoteSelector","exact":"/dev","prefix":"vice)： 与系统周边及储存等相关的一些文件，  通常都集中在","suffix":" 这个目录之下！通常又分为两种： o 区块(block)设备档 "}]}]}
>```
>%%
>*%%PREFIX%%vice)： 与系统周边及储存等相关的一些文件，  通常都集中在%%HIGHLIGHT%% ==/dev== %%POSTFIX%%这个目录之下！通常又分为两种： o 区块(block)设备档*
>%%LINK%%[[#^blmgzophd1q|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^blmgzophd1q


>%%
>```annotation-json
>{"created":"2023-12-03T05:27:17.077Z","text":"不懂","updated":"2023-12-03T05:27:17.077Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":223331,"end":223339},{"type":"TextQuoteSelector","exact":"网络上的数据承接","prefix":" 既然被称为数据接口文件，  想当然尔，这种类型的文件通常被用在","suffix":"了。我们可以启动一个程序来监听客户端的要求，  而客户端就可以透"}]}]}
>```
>%%
>*%%PREFIX%%既然被称为数据接口文件，  想当然尔，这种类型的文件通常被用在%%HIGHLIGHT%% ==网络上的数据承接== %%POSTFIX%%了。我们可以启动一个程序来监听客户端的要求，  而客户端就可以透*
>%%LINK%%[[#^ngwawvyi91|show annotation]]
>%%COMMENT%%
>不懂
>%%TAGS%%
>
^ngwawvyi91


>%%
>```annotation-json
>{"created":"2023-12-03T05:28:08.155Z","updated":"2023-12-03T05:28:08.155Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":223460,"end":223464},{"type":"TextQuoteSelector","exact":"FIFO","prefix":"到这种文件类型了。  数据输送文件(FIFO, pipe)： ","suffix":" 也是一种特殊的文件类型，他主要的目的在解决多个程序同时存取一个"}]}]}
>```
>%%
>*%%PREFIX%%到这种文件类型了。  数据输送文件(FIFO, pipe)：%%HIGHLIGHT%% ==FIFO== %%POSTFIX%%也是一种特殊的文件类型，他主要的目的在解决多个程序同时存取一个*
>%%LINK%%[[#^nnhrhmtpkdt|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^nnhrhmtpkdt


>%%
>```annotation-json
>{"created":"2023-12-03T05:28:59.553Z","text":"与属性有关，而与拓展名无关。跟法语相反，与属性无关，与格式关系最大","updated":"2023-12-03T05:28:59.553Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":223840,"end":223905},{"type":"TextQuoteSelector","exact":"基本上，Linux 的文件是没有所谓的『扩展名』的，我们刚刚就谈过，一个 Linux 文件能不能被执行，与他的第一栏的十个属性有关","prefix":"ocket 来查阅系统上的说明！  Linux 文件扩展名： ","suffix":"，  与文件名根本一点关系也没有。这个观念跟 Windows 的"}]}]}
>```
>%%
>*%%PREFIX%%ocket 来查阅系统上的说明！  Linux 文件扩展名：%%HIGHLIGHT%% ==基本上，Linux 的文件是没有所谓的『扩展名』的，我们刚刚就谈过，一个 Linux 文件能不能被执行，与他的第一栏的十个属性有关== %%POSTFIX%%，  与文件名根本一点关系也没有。这个观念跟 Windows 的*
>%%LINK%%[[#^h3z8ogmu2bb|show annotation]]
>%%COMMENT%%
>与属性有关，而与拓展名无关。跟法语相反，与属性无关，与格式关系最大
>%%TAGS%%
>
^h3z8ogmu2bb


>%%
>```annotation-json
>{"created":"2023-12-03T05:30:24.724Z","updated":"2023-12-03T05:30:24.724Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":224065,"end":224087},{"type":"TextQuoteSelector","exact":"『可执行的权限』以及『具有可执行的程序代码』","prefix":"x ]  即代表这个文件具有可以被执行的能力喔！ Tips 具有","suffix":"是两回事！在  Linux  底下，你可以让一个文本文件，例如我"}]}]}
>```
>%%
>*%%PREFIX%%x ]  即代表这个文件具有可以被执行的能力喔！ Tips 具有%%HIGHLIGHT%% ==『可执行的权限』以及『具有可执行的程序代码』== %%POSTFIX%%是两回事！在  Linux  底下，你可以让一个文本文件，例如我*
>%%LINK%%[[#^7rx4vjocyuk|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^7rx4vjocyuk


>%%
>```annotation-json
>{"created":"2023-12-03T05:30:56.462Z","updated":"2023-12-03T05:30:56.462Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":224252,"end":224264},{"type":"TextQuoteSelector","exact":"可以被执行跟可以执行成功","prefix":"将他的  x  拿掉，那么  cat  将无法被你执行！ 不过，","suffix":"是不一样的～举例来说，在 root 家目录下的  initial"}]}]}
>```
>%%
>*%%PREFIX%%将他的  x  拿掉，那么  cat  将无法被你执行！ 不过，%%HIGHLIGHT%% ==可以被执行跟可以执行成功== %%POSTFIX%%是不一样的～举例来说，在 root 家目录下的  initial*
>%%LINK%%[[#^zxru0w7mm5d|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^zxru0w7mm5d


>%%
>```annotation-json
>{"created":"2023-12-03T05:31:23.383Z","text":"所以只是一种标识","updated":"2023-12-03T05:31:23.383Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":224451,"end":224467},{"type":"TextQuoteSelector","exact":"藉由扩展名来了解该文件是什么东西","prefix":"功，当然就得要看该文件的内容啰～ 虽然如此，不过我们仍然希望可以","suffix":"，所以，  通常我们还是会以适当的扩展名来表示该文件是什么种类的"}]}]}
>```
>%%
>*%%PREFIX%%功，当然就得要看该文件的内容啰～ 虽然如此，不过我们仍然希望可以%%HIGHLIGHT%% ==藉由扩展名来了解该文件是什么东西== %%POSTFIX%%，所以，  通常我们还是会以适当的扩展名来表示该文件是什么种类的*
>%%LINK%%[[#^3cieojbclxj|show annotation]]
>%%COMMENT%%
>所以只是一种标识
>%%TAGS%%
>
^3cieojbclxj


>%%
>```annotation-json
>{"created":"2023-12-03T05:33:03.863Z","text":"一次性执行多条命令，原如","updated":"2023-12-03T05:33:03.863Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":224524,"end":224532},{"type":"TextQuoteSelector","exact":"脚本或批处理文件","prefix":"件是什么种类的。底下有数种常用的扩展名：  *.sh  ：  ","suffix":"  (scripts)，因为批处理文件为使用 shell 写成的"}]}]}
>```
>%%
>*%%PREFIX%%件是什么种类的。底下有数种常用的扩展名：  *.sh  ：%%HIGHLIGHT%% ==脚本或批处理文件== %%POSTFIX%%(scripts)，因为批处理文件为使用 shell 写成的*
>%%LINK%%[[#^2ly1ewmezv5|show annotation]]
>%%COMMENT%%
>一次性执行多条命令，原如
>%%TAGS%%
>
^2ly1ewmezv5


>%%
>```annotation-json
>{"created":"2023-12-03T05:36:42.345Z","text":"是一种特定格式的保存在本地的文件，不要以为是存储在网上的文件，挺抽象的。只是需要浏览器来读取这种格式。","updated":"2023-12-03T05:36:42.345Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":224711,"end":224735},{"type":"TextQuoteSelector","exact":" HTML  语法与  PHP  语法的网页文件","prefix":"名啰！  *.html, *.php：网页相关文件，分别代表 ","suffix":"啰！  .html  的文件可使用网页浏览器来直接开启，至于  "}]}]}
>```
>%%
>*%%PREFIX%%名啰！  *.html, *.php：网页相关文件，分别代表%%HIGHLIGHT%% ==HTML  语法与  PHP  语法的网页文件== %%POSTFIX%%啰！  .html  的文件可使用网页浏览器来直接开启，至于*
>%%LINK%%[[#^upvhabbm4w8|show annotation]]
>%%COMMENT%%
>是一种特定格式的保存在本地的文件，不要以为是存储在网上的文件，挺抽象的。只是需要浏览器来读取这种格式。
>%%TAGS%%
>
^upvhabbm4w8


>%%
>```annotation-json
>{"created":"2023-12-03T05:39:01.704Z","text":"它既是一个文件名，又可以成为命令行中的命令","updated":"2023-12-03T05:39:01.704Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":224953,"end":224956},{"type":"TextQuoteSelector","exact":" ls","prefix":"属性的指令，不过，如果这个文件的权限被修改成无法执行时，  那么","suffix":" 就变成不能执行啰！ 上述的这种问题最常发生在文件传送的过程中。"}]}]}
>```
>%%
>*%%PREFIX%%属性的指令，不过，如果这个文件的权限被修改成无法执行时，  那么%%HIGHLIGHT%% ==ls== %%POSTFIX%%就变成不能执行啰！ 上述的这种问题最常发生在文件传送的过程中。*
>%%LINK%%[[#^187pml3zizt|show annotation]]
>%%COMMENT%%
>它既是一个文件名，又可以成为命令行中的命令
>%%TAGS%%
>
^187pml3zizt


>%%
>```annotation-json
>{"created":"2023-12-03T05:39:36.652Z","updated":"2023-12-03T05:39:36.652Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":225054,"end":225092},{"type":"TextQuoteSelector","exact":"从网络上传送到你的  Linux 系统中，文件的属性与权限确实是会被改变的喔","prefix":"中就是无法执行！呵呵！那么就是可能文件的属性被改变了！不要怀疑，","suffix":"！  Linux 文件长度限制(注 1)： 在 Linux 底"}]}]}
>```
>%%
>*%%PREFIX%%中就是无法执行！呵呵！那么就是可能文件的属性被改变了！不要怀疑，%%HIGHLIGHT%% ==从网络上传送到你的  Linux 系统中，文件的属性与权限确实是会被改变的喔== %%POSTFIX%%！  Linux 文件长度限制(注 1)： 在 Linux 底*
>%%LINK%%[[#^zv28sa85umq|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^zv28sa85umq


>%%
>```annotation-json
>{"created":"2023-12-03T05:44:09.273Z","updated":"2023-12-03T05:44:09.273Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":225220,"end":225228},{"type":"TextQuoteSelector","exact":"255bytes","prefix":"文件的档名长度限制为：  单一文件或目录的最大容许文件名为  ","suffix":"，以一个  ASCII  英文占用一个  bytes  来说，则"}]}]}
>```
>%%
>*%%PREFIX%%文件的档名长度限制为：  单一文件或目录的最大容许文件名为%%HIGHLIGHT%% ==255bytes== %%POSTFIX%%，以一个  ASCII  英文占用一个  bytes  来说，则*
>%%LINK%%[[#^mjij75cxkzo|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^mjij75cxkzo


>%%
>```annotation-json
>{"created":"2023-12-03T07:12:00.155Z","updated":"2023-12-03T07:12:00.155Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":226056,"end":226093},{"type":"TextQuoteSelector","exact":"Filesystem Hierarchy Standard (FHS)标准","prefix":"方法竟然跟你以前学的完全不同吗？很难想象吧～所以，后来就有所谓的","suffix":"的出炉了！ 根据 FHS(注 2)的标准文件指出，他们的主要目的"}]}]}
>```
>%%
>*%%PREFIX%%方法竟然跟你以前学的完全不同吗？很难想象吧～所以，后来就有所谓的%%HIGHLIGHT%% ==Filesystem Hierarchy Standard (FHS)标准== %%POSTFIX%%的出炉了！ 根据 FHS(注 2)的标准文件指出，他们的主要目的*
>%%LINK%%[[#^uwj84jhmwvo|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^uwj84jhmwvo


>%%
>```annotation-json
>{"created":"2023-12-03T07:13:40.548Z","text":"比如说前面已经介绍过的 linux 根目录下通常会有哪些目录","updated":"2023-12-03T07:13:40.548Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":226211,"end":226244},{"type":"TextQuoteSelector","exact":"FHS 的重点在于规范每个特定的目录下应该要放置什么样子的数据而已","prefix":"及想要维护系统的用户，都能够遵循 FHS 的标准。  也就是说，","suffix":"。  这样做好处非常多，因为 Linux 操作系统就能够在既有的"}]}]}
>```
>%%
>*%%PREFIX%%及想要维护系统的用户，都能够遵循 FHS 的标准。  也就是说，%%HIGHLIGHT%% ==FHS 的重点在于规范每个特定的目录下应该要放置什么样子的数据而已== %%POSTFIX%%。  这样做好处非常多，因为 Linux 操作系统就能够在既有的*
>%%LINK%%[[#^48kibgtfffc|show annotation]]
>%%COMMENT%%
>比如说前面已经介绍过的 linux 根目录下通常会有哪些目录
>%%TAGS%%
>
^48kibgtfffc


>%%
>```annotation-json
>{"created":"2023-12-03T07:23:33.872Z","updated":"2023-12-03T07:23:33.872Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":231415,"end":231447},{"type":"TextQuoteSelector","exact":"usr 是 Unix Software Resource 的缩写","prefix":"使用喔！ 很多读者都会误会/usr 为 user 的缩写，其实 ","suffix":"，  也就是『Unix 操作系统软件资源』所放置的目录，而不是用"}]}]}
>```
>%%
>*%%PREFIX%%使用喔！ 很多读者都会误会/usr 为 user 的缩写，其实%%HIGHLIGHT%% ==usr 是 Unix Software Resource 的缩写== %%POSTFIX%%，  也就是『Unix 操作系统软件资源』所放置的目录，而不是用*
>%%LINK%%[[#^sxmdflyenjp|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^sxmdflyenjp


>%%
>```annotation-json
>{"created":"2023-12-03T07:31:18.563Z","updated":"2023-12-03T07:31:18.563Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":236427,"end":236440},{"type":"TextQuoteSelector","exact":"相对于目前路径的文件名写法","prefix":"如  /home/dmtsai/.bashrc；  相对路径：","suffix":"。  例如  ./home/dmtsai  或  ../../h"}]}]}
>```
>%%
>*%%PREFIX%%如  /home/dmtsai/.bashrc；  相对路径：%%HIGHLIGHT%% ==相对于目前路径的文件名写法== %%POSTFIX%%。  例如  ./home/dmtsai  或  ../../h*
>%%LINK%%[[#^iw5zonqn0gb|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^iw5zonqn0gb


>%%
>```annotation-json
>{"created":"2023-12-03T07:31:23.018Z","updated":"2023-12-03T07:31:23.018Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":236371,"end":236391},{"type":"TextQuoteSelector","exact":"由根目录(/)开始写起的文件名或目录名称","prefix":"e)。  这两种文件名/路径的写法依据是这样的：  绝对路径：","suffix":"，  例如  /home/dmtsai/.bashrc；  相"}]}]}
>```
>%%
>*%%PREFIX%%e)。  这两种文件名/路径的写法依据是这样的：  绝对路径：%%HIGHLIGHT%% ==由根目录(/)开始写起的文件名或目录名称== %%POSTFIX%%，  例如  /home/dmtsai/.bashrc；  相*
>%%LINK%%[[#^mb9h4ahcf69|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^mb9h4ahcf69


>%%
>```annotation-json
>{"created":"2023-12-03T07:31:53.615Z","updated":"2023-12-03T07:31:53.615Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":236771,"end":236774},{"type":"TextQuoteSelector","exact":"../","prefix":"也可以使用 ./ 来表示；  .. ：代表上一层目录，也可以 ","suffix":" 来代表。 这个  .  与  ..  目录概念是很重要的，你常"}]}]}
>```
>%%
>*%%PREFIX%%也可以使用 ./ 来表示；  .. ：代表上一层目录，也可以%%HIGHLIGHT%% ==../== %%POSTFIX%%来代表。 这个  .  与  ..  目录概念是很重要的，你常*
>%%LINK%%[[#^dumaqphgdht|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^dumaqphgdht


>%%
>```annotation-json
>{"created":"2023-12-03T11:46:50.938Z","text":"不然会乱删东西","updated":"2023-12-03T11:46:50.938Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":240118,"end":240127},{"type":"TextQuoteSelector","exact":"w 权限不可随便给","prefix":"放目录给任何人浏览时，应该至少也要给予 r 及 x 的权限，但 ","suffix":"；  能否读取到某个文件内容，跟该文件所在的目录权限也有关系 "}]}]}
>```
>%%
>*%%PREFIX%%放目录给任何人浏览时，应该至少也要给予 r 及 x 的权限，但%%HIGHLIGHT%% ==w 权限不可随便给== %%POSTFIX%%；  能否读取到某个文件内容，跟该文件所在的目录权限也有关系*
>%%LINK%%[[#^oiubx74mdad|show annotation]]
>%%COMMENT%%
>不然会乱删东西
>%%TAGS%%
>
^oiubx74mdad


>%%
>```annotation-json
>{"created":"2023-12-03T11:48:11.687Z","text":"之间逗号分隔，不加空格","updated":"2023-12-03T11:48:11.687Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":240737,"end":240751},{"type":"TextQuoteSelector","exact":"u=rwx,g=rx,o=r","prefix":"令？ chmod 754 filename  或  chmod ","suffix":" filename  若我需要更改一个文件的拥有者与群组，该用"}]}]}
>```
>%%
>*%%PREFIX%%令？ chmod 754 filename  或  chmod%%HIGHLIGHT%% ==u=rwx,g=rx,o=r== %%POSTFIX%%filename  若我需要更改一个文件的拥有者与群组，该用*
>%%LINK%%[[#^xyqtjrzyjmk|show annotation]]
>%%COMMENT%%
>之间逗号分隔，不加空格
>%%TAGS%%
>
^xyqtjrzyjmk


>%%
>```annotation-json
>{"created":"2023-12-03T11:51:22.781Z","updated":"2023-12-03T11:51:22.781Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":241805,"end":241815},{"type":"TextQuoteSelector","exact":"操作与管理文件及目录","prefix":"概念以及目录的配置说明。  在这个章节当中，我们就直接来进一步的","suffix":"吧！包括在不同的目录间变换、  建立与删除目录、建立与删除文件，"}]}]}
>```
>%%
>*%%PREFIX%%概念以及目录的配置说明。  在这个章节当中，我们就直接来进一步的%%HIGHLIGHT%% ==操作与管理文件及目录== %%POSTFIX%%吧！包括在不同的目录间变换、  建立与删除目录、建立与删除文件，*
>%%LINK%%[[#^txh7o3kw9bf|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^txh7o3kw9bf


>%%
>```annotation-json
>{"created":"2023-12-03T11:51:33.932Z","text":"都是实际中的常用操作，学会了可以帮你节约大量的时间。","updated":"2023-12-03T11:51:33.932Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":241819,"end":241861},{"type":"TextQuoteSelector","exact":"在不同的目录间变换、  建立与删除目录、建立与删除文件，还有寻找文件、查阅文件内容等","prefix":"在这个章节当中，我们就直接来进一步的操作与管理文件及目录吧！包括","suffix":"等，都会在这个章节作个简单的介绍啊！ 6.1  目录与路径 由前"}]}]}
>```
>%%
>*%%PREFIX%%在这个章节当中，我们就直接来进一步的操作与管理文件及目录吧！包括%%HIGHLIGHT%% ==在不同的目录间变换、  建立与删除目录、建立与删除文件，还有寻找文件、查阅文件内容等== %%POSTFIX%%等，都会在这个章节作个简单的介绍啊！ 6.1  目录与路径 由前*
>%%LINK%%[[#^livhs69n58r|show annotation]]
>%%COMMENT%%
>都是实际中的常用操作，学会了可以帮你节约大量的时间。
>%%TAGS%%
>
^livhs69n58r


>%%
>```annotation-json
>{"created":"2023-12-03T11:52:46.006Z","text":"对这个词粗浅的理解，要建立哪些目录、每个目录里放置什么内容","updated":"2023-12-03T11:52:46.006Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":225892,"end":225896},{"type":"TextQuoteSelector","exact":"目录配置","prefix":"一套标准依据的哩！我们底下就来瞧一瞧。 5.3.1 Linux ","suffix":"的依据--FHS 因为利用 Linux 来开发产品或 distr"}]}]}
>```
>%%
>*%%PREFIX%%一套标准依据的哩！我们底下就来瞧一瞧。 5.3.1 Linux%%HIGHLIGHT%% ==目录配置== %%POSTFIX%%的依据--FHS 因为利用 Linux 来开发产品或 distr*
>%%LINK%%[[#^z1ez4sczlu|show annotation]]
>%%COMMENT%%
>对这个词粗浅的理解，要建立哪些目录、每个目录里放置什么内容
>%%TAGS%%
>
^z1ez4sczlu


>%%
>```annotation-json
>{"created":"2023-12-03T11:56:55.778Z","updated":"2023-12-03T11:56:55.778Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":242206,"end":242230},{"type":"TextQuoteSelector","exact":"绝对路径：路径的写法『一定由根目录  /  写起","prefix":"针对这个议题提过一次，不过，这里不厌其烦的再次的强调一下！  ","suffix":"』，例如：  /usr/share/doc  这个目录。  相"}]}]}
>```
>%%
>*%%PREFIX%%针对这个议题提过一次，不过，这里不厌其烦的再次的强调一下！ %%HIGHLIGHT%% ==绝对路径：路径的写法『一定由根目录  /  写起== %%POSTFIX%%』，例如：  /usr/share/doc  这个目录。  相*
>%%LINK%%[[#^ux1sie6rfp|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ux1sie6rfp


>%%
>```annotation-json
>{"created":"2023-12-03T11:57:21.351Z","updated":"2023-12-03T11:57:21.351Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":242358,"end":242379},{"type":"TextQuoteSelector","exact":"相对路径意指『相对于目前工作目录的路径！』","prefix":"下时，可以写成： 『cd ../man』这就是相对路径的写法啦！","suffix":"  相对路径的用途 那么相对路径与绝对路径有什么了不起呀？喝！"}]}]}
>```
>%%
>*%%PREFIX%%下时，可以写成： 『cd ../man』这就是相对路径的写法啦！%%HIGHLIGHT%% ==相对路径意指『相对于目前工作目录的路径！』== %%POSTFIX%% 相对路径的用途 那么相对路径与绝对路径有什么了不起呀？喝！*
>%%LINK%%[[#^0tatjbc62z2o|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^0tatjbc62z2o


>%%
>```annotation-json
>{"created":"2023-12-03T11:58:14.397Z","text":"采用相对路径就可以更加灵活","updated":"2023-12-03T11:58:14.397Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":242475,"end":242489},{"type":"TextQuoteSelector","exact":"不同的人喜欢安装在不同的目录","prefix":"录，分别是  etc, bin, man  这三个目录，然而由于","suffix":"之下，  假设甲安装的目录是  /usr/local/packa"}]}]}
>```
>%%
>*%%PREFIX%%录，分别是  etc, bin, man  这三个目录，然而由于%%HIGHLIGHT%% ==不同的人喜欢安装在不同的目录== %%POSTFIX%%之下，  假设甲安装的目录是  /usr/local/packa*
>%%LINK%%[[#^4pspo1s5s6q|show annotation]]
>%%COMMENT%%
>采用相对路径就可以更加灵活
>%%TAGS%%
>
^4pspo1s5s6q


>%%
>```annotation-json
>{"created":"2023-12-03T11:58:55.061Z","updated":"2023-12-03T11:58:55.061Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":242951,"end":242964},{"type":"TextQuoteSelector","exact":"绝对路径的正确度要比较好～","prefix":"方便啰！对吧！  绝对路径的用途 但是对于档名的正确性来说，『","suffix":"』。  一般来说，鸟哥会建议你，如果是在写程序  (shell "}]}]}
>```
>%%
>*%%PREFIX%%方便啰！对吧！  绝对路径的用途 但是对于档名的正确性来说，『%%HIGHLIGHT%% ==绝对路径的正确度要比较好～== %%POSTFIX%%』。  一般来说，鸟哥会建议你，如果是在写程序  (shell*
>%%LINK%%[[#^clb5hmyz9aa|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^clb5hmyz9aa


>%%
>```annotation-json
>{"created":"2023-12-03T11:59:55.782Z","updated":"2023-12-03T11:59:55.782Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":243314,"end":243441},{"type":"TextQuoteSelector","exact":".         代表此层目录 ..        代表上一层目录 -         代表前一个工作目录 ~         代表『目前用户身份』所在的家目录 ~account  代表 account 这个用户的家目录(account 是个账号名称)","prefix":" 举例来说，底下这些就是比较特殊的目录，得要用力的记下来才行： ","suffix":" 需要特别注意的是：在所有目录底下都会存在的两个目录，分别是『."}]}]}
>```
>%%
>*%%PREFIX%%举例来说，底下这些就是比较特殊的目录，得要用力的记下来才行：%%HIGHLIGHT%% ==.         代表此层目录 ..        代表上一层目录 -         代表前一个工作目录 ~         代表『目前用户身份』所在的家目录 ~account  代表 account 这个用户的家目录(account 是个账号名称)== %%POSTFIX%%需要特别注意的是：在所有目录底下都会存在的两个目录，分别是『.*
>%%LINK%%[[#^i8du912y86o|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^i8du912y86o


>%%
>```annotation-json
>{"created":"2023-12-03T12:00:31.151Z","text":"所以我们解压文件的时候看到那个名字 .. 的文件夹是不是就是这个东西的具象化","updated":"2023-12-03T12:00:31.151Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":243630,"end":243658},{"type":"TextQuoteSelector","exact":"根目录的上一层(..)与根目录自己(.)是同一个目录。 ","prefix":"，再仔细的查阅，  可发现这两个目录的属性与权限完全一致，这代表","suffix":"底下我们就来谈一谈几个常见的处理目录的指令吧：  cd：变换目"}]}]}
>```
>%%
>*%%PREFIX%%，再仔细的查阅，  可发现这两个目录的属性与权限完全一致，这代表%%HIGHLIGHT%% ==根目录的上一层(..)与根目录自己(.)是同一个目录。== %%POSTFIX%%底下我们就来谈一谈几个常见的处理目录的指令吧：  cd：变换目*
>%%LINK%%[[#^jqdx9b24kvr|show annotation]]
>%%COMMENT%%
>所以我们解压文件的时候看到那个名字 .. 的文件夹是不是就是这个东西的具象化
>%%TAGS%%
>
^jqdx9b24kvr


>%%
>```annotation-json
>{"created":"2023-12-03T12:02:38.985Z","text":"已经迷路了还用相对路径只会越走越远。","updated":"2023-12-03T12:02:38.985Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":244528,"end":244562},{"type":"TextQuoteSelector","exact":"利用相对路径的写法必须要确认你目前的路径才能正确的去到想要去的目录。","prefix":"账号的家目录中。那回到上一层目录可以用『  cd ..  』。 ","suffix":"例如上表当中最后一个例子，  你必须要确认你是在/var/spo"}]}]}
>```
>%%
>*%%PREFIX%%账号的家目录中。那回到上一层目录可以用『  cd ..  』。%%HIGHLIGHT%% ==利用相对路径的写法必须要确认你目前的路径才能正确的去到想要去的目录。== %%POSTFIX%%例如上表当中最后一个例子，  你必须要确认你是在/var/spo*
>%%LINK%%[[#^1dpcjwxm75e|show annotation]]
>%%COMMENT%%
>已经迷路了还用相对路径只会越走越远。
>%%TAGS%%
>
^1dpcjwxm75e


>%%
>```annotation-json
>{"created":"2023-12-03T12:03:31.797Z","updated":"2023-12-03T12:03:31.797Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":244772,"end":244794},{"type":"TextQuoteSelector","exact":"家目录还有一个代码，那就是『  ~  』符号","prefix":" 当中，就已经有指出当前目录了，  刚登入时会到自己的家目录，而","suffix":"！  例如上面的例子可以发现，使用『  cd ~  』可以回到个"}]}]}
>```
>%%
>*%%PREFIX%%当中，就已经有指出当前目录了，  刚登入时会到自己的家目录，而%%HIGHLIGHT%% ==家目录还有一个代码，那就是『  ~  』符号== %%POSTFIX%%！  例如上面的例子可以发现，使用『  cd ~  』可以回到个*
>%%LINK%%[[#^0c6j3tiqntm8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^0c6j3tiqntm8


>%%
>```annotation-json
>{"created":"2023-12-03T12:03:45.608Z","updated":"2023-12-03T12:03:45.608Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":244857,"end":244886},{"type":"TextQuoteSelector","exact":"仅输入  cd  时，代表的就是『  cd ~  』的意思","prefix":"个人的家目录里头去呢！  另外，针对  cd  的使用方法，如果","suffix":"喔～  亦即是会回到自己的家目录啦！而那个『  cd -  』比"}]}]}
>```
>%%
>*%%PREFIX%%个人的家目录里头去呢！  另外，针对  cd  的使用方法，如果%%HIGHLIGHT%% ==仅输入  cd  时，代表的就是『  cd ~  』的意思== %%POSTFIX%%喔～  亦即是会回到自己的家目录啦！而那个『  cd -  』比*
>%%LINK%%[[#^n2s442wjcxf|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^n2s442wjcxf


>%%
>```annotation-json
>{"created":"2023-12-03T12:03:50.400Z","updated":"2023-12-03T12:03:50.400Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":244713,"end":244717},{"type":"TextQuoteSelector","exact":"提示字符","prefix":"cd /var/spool/postfix  啰～ 其实，我们的","suffix":"，亦即那个  [root@study ~]#  当中，就已经有指"}]}]}
>```
>%%
>*%%PREFIX%%cd /var/spool/postfix  啰～ 其实，我们的%%HIGHLIGHT%% ==提示字符== %%POSTFIX%%，亦即那个  [root@study ~]#  当中，就已经有指*
>%%LINK%%[[#^j2p16sd7bff|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^j2p16sd7bff


>%%
>```annotation-json
>{"created":"2023-12-03T12:04:19.088Z","updated":"2023-12-03T12:04:19.088Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":245607,"end":245640},{"type":"TextQuoteSelector","exact":"pwd 是 Print Working Directory 的缩写","prefix":"的选项后，会不以连结文件的数据显示，而是显示正确的完整路径啊！ ","suffix":"，也就是显示目前所在目录的指令，  例如在上个表格最后的目录是/"}]}]}
>```
>%%
>*%%PREFIX%%的选项后，会不以连结文件的数据显示，而是显示正确的完整路径啊！%%HIGHLIGHT%% ==pwd 是 Print Working Directory 的缩写== %%POSTFIX%%，也就是显示目前所在目录的指令，  例如在上个表格最后的目录是/*
>%%LINK%%[[#^sbat4g8pxb9|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^sbat4g8pxb9


>%%
>```annotation-json
>{"created":"2023-12-03T12:06:18.026Z","text":"显示文件所在地址而非快捷方式所在地址","updated":"2023-12-03T12:06:18.026Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":245851,"end":245853},{"type":"TextQuoteSelector","exact":"-P","prefix":"道你的所在目录啰！免得搞错目录，结果... 其实有趣的是那个  ","suffix":"  的选项啦！他可以让我们取得正确的目录名称，而不是以链接文件的"}]}]}
>```
>%%
>*%%PREFIX%%道你的所在目录啰！免得搞错目录，结果... 其实有趣的是那个%%HIGHLIGHT%% ==-P== %%POSTFIX%%的选项啦！他可以让我们取得正确的目录名称，而不是以链接文件的*
>%%LINK%%[[#^lyakrbdlnde|show annotation]]
>%%COMMENT%%
>显示文件所在地址而非快捷方式所在地址
>%%TAGS%%
>
^lyakrbdlnde


>%%
>```annotation-json
>{"created":"2023-12-03T12:07:42.165Z","text":"递归建立，一个一个将你没建的目录建出来。","updated":"2023-12-03T12:07:42.165Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":246486,"end":246505},{"type":"TextQuoteSelector","exact":"-p 的选项，可以自行帮你建立多层目录","prefix":"原来是要建 test4 上层没先建 test3 之故！加了这个 ","suffix":"！  范例：建立权限为 rwx--x--x 的目录 [root@"}]}]}
>```
>%%
>*%%PREFIX%%原来是要建 test4 上层没先建 test3 之故！加了这个%%HIGHLIGHT%% ==-p 的选项，可以自行帮你建立多层目录== %%POSTFIX%%！  范例：建立权限为 rwx--x--x 的目录 [root@*
>%%LINK%%[[#^coq3t4ikt7w|show annotation]]
>%%COMMENT%%
>递归建立，一个一个将你没建的目录建出来。
>%%TAGS%%
>
^coq3t4ikt7w


>%%
>```annotation-json
>{"created":"2023-12-03T12:08:51.805Z","updated":"2023-12-03T12:08:51.805Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":246757,"end":246782},{"type":"TextQuoteSelector","exact":"没有加上 -m 来强制设定属性，系统会使用默认属性","prefix":"n  4 19:05 test2 # 仔细看上面的权限部分，如果","suffix":"。 # 那么你的默认属性为何？这要透过底下介绍的 umask 才"}]}]}
>```
>%%
>*%%PREFIX%%n  4 19:05 test2 # 仔细看上面的权限部分，如果%%HIGHLIGHT%% ==没有加上 -m 来强制设定属性，系统会使用默认属性== %%POSTFIX%%。 # 那么你的默认属性为何？这要透过底下介绍的 umask 才*
>%%LINK%%[[#^ma590go315b|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ma590go315b


>%%
>```annotation-json
>{"created":"2023-12-03T12:10:16.860Z","updated":"2023-12-03T12:10:16.860Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":248280,"end":248334},{"type":"TextQuoteSelector","exact":"被删除的目录里面必定不能存在其他的目录或文件！ 这也是所谓的空的目录(empty directory)的意思","prefix":" test  』即可！请注意呦！目录需要一层一层的删除才行！而且","suffix":"啊！那如果要将所有目录下的东西都杀掉呢？！  这个时候就必须使用"}]}]}
>```
>%%
>*%%PREFIX%%test  』即可！请注意呦！目录需要一层一层的删除才行！而且%%HIGHLIGHT%% ==被删除的目录里面必定不能存在其他的目录或文件！ 这也是所谓的空的目录(empty directory)的意思== %%POSTFIX%%啊！那如果要将所有目录下的东西都杀掉呢？！  这个时候就必须使用*
>%%LINK%%[[#^6t37t7gjanu|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^6t37t7gjanu


>%%
>```annotation-json
>{"created":"2023-12-03T12:10:52.266Z","text":"什么叫上层的目录","updated":"2023-12-03T12:10:52.266Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":248428,"end":248433},{"type":"TextQuoteSelector","exact":"上层的目录","prefix":"ir  比较不危险！你也可以尝试以  -p  的选项加入，来删除","suffix":"喔！ 6.1.3  关于执行文件路径的变量：  $PATH 经过"}]}]}
>```
>%%
>*%%PREFIX%%ir  比较不危险！你也可以尝试以  -p  的选项加入，来删除%%HIGHLIGHT%% ==上层的目录== %%POSTFIX%%喔！ 6.1.3  关于执行文件路径的变量：  $PATH 经过*
>%%LINK%%[[#^cv30t4lswq5|show annotation]]
>%%COMMENT%%
>什么叫上层的目录
>%%TAGS%%
>
^cv30t4lswq5


>%%
>```annotation-json
>{"created":"2023-12-03T12:13:08.396Z","text":"得益于 FHS ，各个系统的环境变量应该还算统一。","updated":"2023-12-03T12:13:08.396Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":248664,"end":248761},{"type":"TextQuoteSelector","exact":"系统会依照 PATH 的设定去每个 PATH 定义的目录下搜寻文件名为 ls 的可执行文件，  如果在 PATH 定义的目录中含有多个文件名为 ls 的可执行文件，那么先搜寻到的同名指令先被执行","prefix":"帮助所致呀！ 当我们在执行一个指令的时候，举例来说『ls』好了，","suffix":"！ 现在，请下达『echo $PATH』来看看到底有哪些目录被定"}]}]}
>```
>%%
>*%%PREFIX%%帮助所致呀！ 当我们在执行一个指令的时候，举例来说『ls』好了，%%HIGHLIGHT%% ==系统会依照 PATH 的设定去每个 PATH 定义的目录下搜寻文件名为 ls 的可执行文件，  如果在 PATH 定义的目录中含有多个文件名为 ls 的可执行文件，那么先搜寻到的同名指令先被执行== %%POSTFIX%%！ 现在，请下达『echo $PATH』来看看到底有哪些目录被定*
>%%LINK%%[[#^b46hhv8to7t|show annotation]]
>%%COMMENT%%
>得益于 FHS ，各个系统的环境变量应该还算统一。
>%%TAGS%%
>
^b46hhv8to7t


>%%
>```annotation-json
>{"created":"2023-12-03T12:20:46.347Z","updated":"2023-12-03T12:20:46.347Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":248769,"end":248844},{"type":"TextQuoteSelector","exact":"『echo $PATH』来看看到底有哪些目录被定义出来了？  echo 有『显示、印出』的意思，而  PATH  前面加的  $  表示后面接的是变量","prefix":"s 的可执行文件，那么先搜寻到的同名指令先被执行！ 现在，请下达","suffix":"，所以会显示出目前的  PATH  ！ 范例：先用 root 的"}]}]}
>```
>%%
>*%%PREFIX%%s 的可执行文件，那么先搜寻到的同名指令先被执行！ 现在，请下达%%HIGHLIGHT%% ==『echo $PATH』来看看到底有哪些目录被定义出来了？  echo 有『显示、印出』的意思，而  PATH  前面加的  $  表示后面接的是变量== %%POSTFIX%%，所以会显示出目前的  PATH  ！ 范例：先用 root 的*
>%%LINK%%[[#^iym1vsp59kn|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^iym1vsp59kn


>%%
>```annotation-json
>{"created":"2023-12-03T12:22:37.192Z","text":"命令行遇到可执行文件，如果你没有提供绝对地址的话，搜索的是环境变量中的目录，而非当前目录。","updated":"2023-12-03T12:22:37.192Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":250118,"end":250174},{"type":"TextQuoteSelector","exact":"如果想要让 root 在任何目录均可执行/root 底下的 ls，那么就将/root 加入 PATH 当中即可。","prefix":" <==因为在 /root 目录下，就用./ls 来指定 (3)","suffix":"  加入的方法很简单，就像底下这样： [root@study ~"}]}]}
>```
>%%
>*%%PREFIX%%<==因为在 /root 目录下，就用./ls 来指定 (3)%%HIGHLIGHT%% ==如果想要让 root 在任何目录均可执行/root 底下的 ls，那么就将/root 加入 PATH 当中即可。== %%POSTFIX%%加入的方法很简单，就像底下这样： [root@study ~*
>%%LINK%%[[#^3gwvse91s0a|show annotation]]
>%%COMMENT%%
>命令行遇到可执行文件，如果你没有提供绝对地址的话，搜索的是环境变量中的目录，而非当前目录。
>%%TAGS%%
>
^3gwvse91s0a


>%%
>```annotation-json
>{"created":"2023-12-03T12:24:50.277Z","updated":"2023-12-03T12:24:50.277Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":251102,"end":251108},{"type":"TextQuoteSelector","exact":"为了安全起见","prefix":"是经常会被用到的 ls 时，那『中标』的机率就更高了！  所以，","suffix":"，不建议将『.』加入 PATH 的搜寻目录中。 而由上面的几个例"}]}]}
>```
>%%
>*%%PREFIX%%是经常会被用到的 ls 时，那『中标』的机率就更高了！  所以，%%HIGHLIGHT%% ==为了安全起见== %%POSTFIX%%，不建议将『.』加入 PATH 的搜寻目录中。 而由上面的几个例*
>%%LINK%%[[#^neous6rt1i|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^neous6rt1i


>%%
>```annotation-json
>{"created":"2023-12-03T12:26:35.747Z","updated":"2023-12-03T12:26:35.747Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":251422,"end":251452},{"type":"TextQuoteSelector","exact":"『显示属性』、  『拷贝』、『删除文件』及『移动文件或目录』","prefix":"再来讨论一下关于文件的一些基本管理吧！文件与目录的管理上，不外乎","suffix":"等等，由于文件与目录的管理在  Linux  当中是很重要的， "}]}]}
>```
>%%
>*%%PREFIX%%再来讨论一下关于文件的一些基本管理吧！文件与目录的管理上，不外乎%%HIGHLIGHT%% ==『显示属性』、  『拷贝』、『删除文件』及『移动文件或目录』== %%POSTFIX%%等等，由于文件与目录的管理在  Linux  当中是很重要的，*
>%%LINK%%[[#^tsn97ackfxl|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^tsn97ackfxl


>%%
>```annotation-json
>{"created":"2023-12-03T12:28:09.118Z","updated":"2023-12-03T12:28:09.118Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":252647,"end":252663},{"type":"TextQuoteSelector","exact":"以蓝色显示目录及白色显示一般文件","prefix":" 你下达『  ls /etc  』之后，只有经过排序的文件名以及","suffix":"，如此而已。 那如果我还想要加入其他的显示信息时，可以加入上头提"}]}]}
>```
>%%
>*%%PREFIX%%你下达『  ls /etc  』之后，只有经过排序的文件名以及%%HIGHLIGHT%% ==以蓝色显示目录及白色显示一般文件== %%POSTFIX%%，如此而已。 那如果我还想要加入其他的显示信息时，可以加入上头提*
>%%LINK%%[[#^i3m39uoa7bk|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^i3m39uoa7bk


>%%
>```annotation-json
>{"created":"2023-12-03T12:28:13.361Z","updated":"2023-12-03T12:28:13.361Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":252594,"end":252604},{"type":"TextQuoteSelector","exact":"文件名代表的颜色显示","prefix":"ls  时，默认显示的只有：非隐藏档的档名、  以档名进行排序及","suffix":"如此而已。举例来说，  你下达『  ls /etc  』之后，只"}]}]}
>```
>%%
>*%%PREFIX%%ls  时，默认显示的只有：非隐藏档的档名、  以档名进行排序及%%HIGHLIGHT%% ==文件名代表的颜色显示== %%POSTFIX%%如此而已。举例来说，  你下达『  ls /etc  』之后，只*
>%%LINK%%[[#^3r2swksm42f|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^3r2swksm42f


>%%
>```annotation-json
>{"created":"2023-12-03T12:31:42.974Z","text":"所以可供选择展示的参数也很多","updated":"2023-12-03T12:31:42.974Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":252519,"end":252532},{"type":"TextQuoteSelector","exact":"文件所记录的信息实在是太多","prefix":"要知道文件或者是目录的相关信息啊～  不过，我们 Linux 的","suffix":"了，ls  没有需要全部都列出来呢～ 所以，当你只有下达  ls"}]}]}
>```
>%%
>*%%PREFIX%%要知道文件或者是目录的相关信息啊～  不过，我们 Linux 的%%HIGHLIGHT%% ==文件所记录的信息实在是太多== %%POSTFIX%%了，ls  没有需要全部都列出来呢～ 所以，当你只有下达  ls*
>%%LINK%%[[#^gbmnp8nvfm|show annotation]]
>%%COMMENT%%
>所以可供选择展示的参数也很多
>%%TAGS%%
>
^gbmnp8nvfm


>%%
>```annotation-json
>{"created":"2023-12-03T12:35:33.878Z","text":"防脑瘫","updated":"2023-12-03T12:35:33.878Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":256158,"end":256161},{"type":"TextQuoteSelector","exact":"-i ","prefix":"e)的意思，若目标文件已经存在且无法开启，则移除后再尝试一次； ","suffix":" ：若目标文件(destination)已经存在时，在覆盖时会先"}]}]}
>```
>%%
>*%%PREFIX%%e)的意思，若目标文件已经存在且无法开启，则移除后再尝试一次；%%HIGHLIGHT%% ==-i== %%POSTFIX%%：若目标文件(destination)已经存在时，在覆盖时会先*
>%%LINK%%[[#^d2addgc8sg7|show annotation]]
>%%COMMENT%%
>防脑瘫
>%%TAGS%%
>
^d2addgc8sg7


>%%
>```annotation-json
>{"created":"2023-12-03T12:37:39.901Z","text":"复制之后将文件变成自己的了，windows中好像很少有这种概念。","updated":"2023-12-03T12:37:39.901Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":257697,"end":257766},{"type":"TextQuoteSelector","exact":"希望复制到的数据最后是我们自己的，所以，在预设的条件中，  cp  的来源档与目的档的权限是不同的，目的档的拥有者通常会是指令操作者本身。","prefix":"须要有  read  的权限才行啊！  ^_^)  时，  总是","suffix":"举例来说，  上面的范例二中，由于我是  root  的身份，因"}]}]}
>```
>%%
>*%%PREFIX%%须要有  read  的权限才行啊！  ^_^)  时，  总是%%HIGHLIGHT%% ==希望复制到的数据最后是我们自己的，所以，在预设的条件中，  cp  的来源档与目的档的权限是不同的，目的档的拥有者通常会是指令操作者本身。== %%POSTFIX%%举例来说，  上面的范例二中，由于我是  root  的身份，因*
>%%LINK%%[[#^6blxyol2l6|show annotation]]
>%%COMMENT%%
>复制之后将文件变成自己的了，windows中好像很少有这种概念。
>%%TAGS%%
>
^6blxyol2l6


>%%
>```annotation-json
>{"created":"2023-12-03T12:39:14.862Z","text":"recurrence ， 但是很怪，之前命令的递归又是-p","updated":"2023-12-03T12:39:14.862Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":256289,"end":256310},{"type":"TextQuoteSelector","exact":"-r  ：递归持续复制，用于目录的复制行为","prefix":"权限、用户、时间)一起复制过去，而非使用默认属性(备份常用)； ","suffix":"；(常用) -s  ：复制成为符号链接文件 (symbolic "}]}]}
>```
>%%
>*%%PREFIX%%权限、用户、时间)一起复制过去，而非使用默认属性(备份常用)；%%HIGHLIGHT%% ==-r  ：递归持续复制，用于目录的复制行为== %%POSTFIX%%；(常用) -s  ：复制成为符号链接文件 (symbolic*
>%%LINK%%[[#^02z2zktsn7dq|show annotation]]
>%%COMMENT%%
>recurrence ， 但是很怪，之前命令的递归又是-p
>%%TAGS%%
>
^02z2zktsn7dq


>%%
>```annotation-json
>{"created":"2023-12-03T12:40:39.255Z","text":"*标识文件开头是 bashrc","updated":"2023-12-03T12:40:39.255Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":258561,"end":258568},{"type":"TextQuoteSelector","exact":"bashrc*","prefix":"c_hlink [root@study tmp]# ls -l ","suffix":" -rw-r--r--. 2 root root 176 Jun"}]}]}
>```
>%%
>*%%PREFIX%%c_hlink [root@study tmp]# ls -l%%HIGHLIGHT%% ==bashrc*== %%POSTFIX%%-rw-r--r--. 2 root root 176 Jun*
>%%LINK%%[[#^e95kjfftmqr|show annotation]]
>%%COMMENT%%
>*标识文件开头是 bashrc
>%%TAGS%%
>
^e95kjfftmqr


>%%
>```annotation-json
>{"created":"2023-12-03T12:43:22.509Z","text":"强迫这个文件变成你的，切断与源文件的关联，防止你打什么歪主意。","updated":"2023-12-03T12:43:22.509Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":260389,"end":260437},{"type":"TextQuoteSelector","exact":"原本  dmtsai  身份无法进行的动作，即使加上  -a  选项，也是无法达成完整复制权限的","prefix":"wtmp 的相关权限与时间等属性，  但是与拥有者、群组相关的，","suffix":"！ 总之，由于  cp  有种种的文件属性与权限的特性，所以，在"}]}]}
>```
>%%
>*%%PREFIX%%wtmp 的相关权限与时间等属性，  但是与拥有者、群组相关的，%%HIGHLIGHT%% ==原本  dmtsai  身份无法进行的动作，即使加上  -a  选项，也是无法达成完整复制权限的== %%POSTFIX%%！ 总之，由于  cp  有种种的文件属性与权限的特性，所以，在*
>%%LINK%%[[#^tnwvxp7ajlo|show annotation]]
>%%COMMENT%%
>强迫这个文件变成你的，切断与源文件的关联，防止你打什么歪主意。
>%%TAGS%%
>
^tnwvxp7ajlo


>%%
>```annotation-json
>{"created":"2023-12-03T12:44:42.115Z","updated":"2023-12-03T12:44:42.115Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":260979,"end":260998},{"type":"TextQuoteSelector","exact":"星号，代表的是 0 到无穷多个任意字符","prefix":"study tmp]# rm -i bashrc* # 注意那个","suffix":"喔！很好用的东西！  范例三：将 cp 范例中所建立的 /tmp"}]}]}
>```
>%%
>*%%PREFIX%%study tmp]# rm -i bashrc* # 注意那个%%HIGHLIGHT%% ==星号，代表的是 0 到无穷多个任意字符== %%POSTFIX%%喔！很好用的东西！  范例三：将 cp 范例中所建立的 /tmp*
>%%LINK%%[[#^qhwh3j04gb8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^qhwh3j04gb8


>%%
>```annotation-json
>{"created":"2023-12-03T12:46:46.552Z","text":"特定的文件名开头会造成误判","updated":"2023-12-03T12:46:46.552Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":262384,"end":262386},{"type":"TextQuoteSelector","exact":"误判","prefix":"选项，因此，单纯的使用『  rm -aaa-  』系统的指令就会","suffix":"啦！  那如果使用后面会谈到的正规表示法时，还是会出问题的！所以"}]}]}
>```
>%%
>*%%PREFIX%%选项，因此，单纯的使用『  rm -aaa-  』系统的指令就会%%HIGHLIGHT%% ==误判== %%POSTFIX%%啦！  那如果使用后面会谈到的正规表示法时，还是会出问题的！所以*
>%%LINK%%[[#^ghxwinbrqmf|show annotation]]
>%%COMMENT%%
>特定的文件名开头会造成误判
>%%TAGS%%
>
^ghxwinbrqmf


>%%
>```annotation-json
>{"created":"2023-12-03T12:47:29.832Z","updated":"2023-12-03T12:47:29.832Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":263448,"end":263470},{"type":"TextQuoteSelector","exact":"很轻易的使用  mv  来变更一个文件的档名","prefix":"看看是否需要搬移啰！  另外一个用途就是『变更档名！』，我们可以","suffix":"呢！不过，在  Linux  才有的指令当中，有个 rename"}]}]}
>```
>%%
>*%%PREFIX%%看看是否需要搬移啰！  另外一个用途就是『变更档名！』，我们可以%%HIGHLIGHT%% ==很轻易的使用  mv  来变更一个文件的档名== %%POSTFIX%%呢！不过，在  Linux  才有的指令当中，有个 rename*
>%%LINK%%[[#^es4d0pftt27|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^es4d0pftt27


>%%
>```annotation-json
>{"created":"2023-12-03T12:47:56.434Z","text":"毕竟只有目录才放得下多个文件","updated":"2023-12-03T12:47:56.434Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":263284,"end":263311},{"type":"TextQuoteSelector","exact":"多个来源文件或目录，则最后一个目标文件一定是『目录！』","prefix":"hrc1 bashrc2 mvtest2 # 注意到这边，如果有","suffix":" # 意思是说，将所有的数据移动到该目录的意思！ 这是搬移  ("}]}]}
>```
>%%
>*%%PREFIX%%hrc1 bashrc2 mvtest2 # 注意到这边，如果有%%HIGHLIGHT%% ==多个来源文件或目录，则最后一个目标文件一定是『目录！』== %%POSTFIX%%# 意思是说，将所有的数据移动到该目录的意思！ 这是搬移  (*
>%%LINK%%[[#^t2f8je801jd|show annotation]]
>%%COMMENT%%
>毕竟只有目录才放得下多个文件
>%%TAGS%%
>
^t2f8je801jd


>%%
>```annotation-json
>{"created":"2023-12-03T12:48:25.796Z","text":"后面两个加起来构成了文件的完整档名。\n例如辨别一个人需要他的完整住址和姓名。","updated":"2023-12-03T12:48:25.796Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":263578,"end":263602},{"type":"TextQuoteSelector","exact":"每个文件的完整档名包含了前面的目录与最终的文件名","prefix":"也是挺有趣的指令喔！ 6.2.3  取得路径的文件名与目录名称 ","suffix":"，而每个档名的长度都可以到达  255  个字符耶！  那么你怎"}]}]}
>```
>%%
>*%%PREFIX%%也是挺有趣的指令喔！ 6.2.3  取得路径的文件名与目录名称%%HIGHLIGHT%% ==每个文件的完整档名包含了前面的目录与最终的文件名== %%POSTFIX%%，而每个档名的长度都可以到达  255  个字符耶！  那么你怎*
>%%LINK%%[[#^w4of09vl3ba|show annotation]]
>%%COMMENT%%
>后面两个加起来构成了文件的完整档名。
>例如辨别一个人需要他的完整住址和姓名。
>%%TAGS%%
>
^w4of09vl3ba


>%%
>```annotation-json
>{"created":"2023-12-03T12:48:59.453Z","text":"文件名","updated":"2023-12-03T12:48:59.453Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":263640,"end":263642},{"type":"TextQuoteSelector","exact":"档名","prefix":"的长度都可以到达  255  个字符耶！  那么你怎么知道那个是","suffix":"？那个是目录名？嘿嘿！就是利用斜线  (/)  来分辨啊！  其"}]}]}
>```
>%%
>*%%PREFIX%%的长度都可以到达  255  个字符耶！  那么你怎么知道那个是%%HIGHLIGHT%% ==档名== %%POSTFIX%%？那个是目录名？嘿嘿！就是利用斜线  (/)  来分辨啊！  其*
>%%LINK%%[[#^qmy4ftz36zb|show annotation]]
>%%COMMENT%%
>文件名
>%%TAGS%%
>
^qmy4ftz36zb


>%%
>```annotation-json
>{"created":"2023-12-03T12:49:02.716Z","text":"所在的目录的名字","updated":"2023-12-03T12:49:02.716Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":263646,"end":263649},{"type":"TextQuoteSelector","exact":"目录名","prefix":"到达  255  个字符耶！  那么你怎么知道那个是档名？那个是","suffix":"？嘿嘿！就是利用斜线  (/)  来分辨啊！  其实，取得文件名"}]}]}
>```
>%%
>*%%PREFIX%%到达  255  个字符耶！  那么你怎么知道那个是档名？那个是%%HIGHLIGHT%% ==目录名== %%POSTFIX%%？嘿嘿！就是利用斜线  (/)  来分辨啊！  其实，取得文件名*
>%%LINK%%[[#^vlfxdq7nxto|show annotation]]
>%%COMMENT%%
>所在的目录的名字
>%%TAGS%%
>
^vlfxdq7nxto


>%%
>```annotation-json
>{"created":"2023-12-03T15:22:36.234Z","updated":"2023-12-03T15:22:36.234Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":264213,"end":264227},{"type":"TextQuoteSelector","exact":"tac 是 cat 的倒着写","prefix":"行开始显示文件内容  tac  从最后一行开始显示，可以看出 ","suffix":"！  nl   显示的时候，顺道输出行号！  more 一页"}]}]}
>```
>%%
>*%%PREFIX%%行开始显示文件内容  tac  从最后一行开始显示，可以看出%%HIGHLIGHT%% ==tac 是 cat 的倒着写== %%POSTFIX%%！  nl   显示的时候，顺道输出行号！  more 一页*
>%%LINK%%[[#^kvl2d0uyjk|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^kvl2d0uyjk


>%%
>```annotation-json
>{"created":"2023-12-05T10:30:10.949Z","updated":"2023-12-05T10:30:10.949Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":299817,"end":299842},{"type":"TextQuoteSelector","exact":"该目录要具有  w,x  的权限，重点在  w  ","prefix":"使用者可以建立一个文件的基本权限为何？  目录所需权限：用户在","suffix":"啦！ 五、让用户进入某目录并执行该目录下的某个指令之基本权限为何"}]}]}
>```
>%%
>*%%PREFIX%%使用者可以建立一个文件的基本权限为何？  目录所需权限：用户在%%HIGHLIGHT%% ==该目录要具有  w,x  的权限，重点在  w== %%POSTFIX%%啦！ 五、让用户进入某目录并执行该目录下的某个指令之基本权限为何*
>%%LINK%%[[#^x2ggq1aauo8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^x2ggq1aauo8


>%%
>```annotation-json
>{"created":"2023-12-05T10:32:37.909Z","text":"不能只有 w ，但是话说为什么我会有这么奇怪的想法呢。","updated":"2023-12-05T10:32:37.909Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":299758,"end":299779},{"type":"TextQuoteSelector","exact":"使用者对该文件至少要有  r, w  权限","prefix":"户在该文件所在的目录至少要有  x  权限；  文件所需权限：","suffix":" 四、让一个使用者可以建立一个文件的基本权限为何？  目录所需"}]}]}
>```
>%%
>*%%PREFIX%%户在该文件所在的目录至少要有  x  权限；  文件所需权限：%%HIGHLIGHT%% ==使用者对该文件至少要有  r, w  权限== %%POSTFIX%%四、让一个使用者可以建立一个文件的基本权限为何？  目录所需*
>%%LINK%%[[#^j97orwuzt3|show annotation]]
>%%COMMENT%%
>不能只有 w ，但是话说为什么我会有这么奇怪的想法呢。
>%%TAGS%%
>
^j97orwuzt3


>%%
>```annotation-json
>{"created":"2023-12-05T10:33:18.817Z","text":"复制只需要 read 文件的权力。\n就想象你只需要知道文件里写了什么，但是不需要对它作出修改，就可以复制一个文件啦。","updated":"2023-12-05T10:33:18.817Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":300133,"end":300141},{"type":"TextQuoteSelector","exact":"需要有 r 权限","prefix":"：  dir1 ：至少需要有 x 权限；  file1：至少","suffix":"；  dir2 ：至少需要有 w, x 权限。  例题： 有一"}]}]}
>```
>%%
>*%%PREFIX%%：  dir1 ：至少需要有 x 权限；  file1：至少%%HIGHLIGHT%% ==需要有 r 权限== %%POSTFIX%%；  dir2 ：至少需要有 w, x 权限。  例题： 有一*
>%%LINK%%[[#^zgden9qpie|show annotation]]
>%%COMMENT%%
>复制只需要 read 文件的权力。
>就想象你只需要知道文件里写了什么，但是不需要对它作出修改，就可以复制一个文件啦。
>%%TAGS%%
>
^zgden9qpie


>%%
>```annotation-json
>{"created":"2023-12-05T11:10:15.372Z","updated":"2023-12-05T11:10:15.372Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":306096,"end":306115},{"type":"TextQuoteSelector","exact":"制作文件系统，包括分区、格式化与挂载等","prefix":" 当预设文件系统了！这也得了解一下。  在本章我们的重点在于如何","suffix":"，是很重要的一个章节喔！ 7.1  认识  Linux  文件系"}]}]}
>```
>%%
>*%%PREFIX%%当预设文件系统了！这也得了解一下。  在本章我们的重点在于如何%%HIGHLIGHT%% ==制作文件系统，包括分区、格式化与挂载等== %%POSTFIX%%，是很重要的一个章节喔！ 7.1  认识  Linux  文件系*
>%%LINK%%[[#^e7t04b05zln|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^e7t04b05zln


>%%
>```annotation-json
>{"created":"2023-12-05T11:13:45.778Z","text":"最大的是盘面；\n盘面上一个个圆环称为磁道，注意磁道是一整个环噢；\n扇区则是将磁道一刀刀的切开的一个个扇环，是这三个概念里最小的那个。\n磁柱我的理解是很多个扇区叠起来形成的柱体，毕竟你有很多盘面嘛。但这好像跟书上的说法有出入。","updated":"2023-12-05T11:13:45.778Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":102637,"end":102671},{"type":"TextQuoteSelector","exact":"磁盘盘上面又可细分出扇区(Sector)与磁道(Track)两种单位","prefix":"磁盘读取头与主轴马达所组成，  而数据的写入其实是在磁盘盘上面。","suffix":"，  其中扇区的物理量设计有两种大小，分别是  512bytes"}]}]}
>```
>%%
>*%%PREFIX%%磁盘读取头与主轴马达所组成，  而数据的写入其实是在磁盘盘上面。%%HIGHLIGHT%% ==磁盘盘上面又可细分出扇区(Sector)与磁道(Track)两种单位== %%POSTFIX%%，  其中扇区的物理量设计有两种大小，分别是  512bytes*
>%%LINK%%[[#^kdwk623ywi|show annotation]]
>%%COMMENT%%
>最大的是盘面；
>盘面上一个个圆环称为磁道，注意磁道是一整个环噢；
>扇区则是将磁道一刀刀的切开的一个个扇环，是这三个概念里最小的那个。
>磁柱我的理解是很多个扇区叠起来形成的柱体，毕竟你有很多盘面嘛。但这好像跟书上的说法有出入。
>%%TAGS%%
>#硬盘
^kdwk623ywi


>%%
>```annotation-json
>{"created":"2023-12-05T11:18:07.112Z","updated":"2023-12-05T11:18:07.112Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":102834,"end":102858},{"type":"TextQuoteSelector","exact":"MBR (Master Boot Record)","prefix":"盘的重要信息！  早期磁盘第一个扇区里面含有的重要信息我们称为 ","suffix":"  格式，但是由于近年来磁盘的容量不断扩大，造成读写上的一些困扰"}]}]}
>```
>%%
>*%%PREFIX%%盘的重要信息！  早期磁盘第一个扇区里面含有的重要信息我们称为%%HIGHLIGHT%% ==MBR (Master Boot Record)== %%POSTFIX%%格式，但是由于近年来磁盘的容量不断扩大，造成读写上的一些困扰*
>%%LINK%%[[#^0a2w1j9rn1yx|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#硬盘
^0a2w1j9rn1yx


>%%
>```annotation-json
>{"created":"2023-12-05T11:18:17.609Z","updated":"2023-12-05T11:18:17.609Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":102949,"end":102975},{"type":"TextQuoteSelector","exact":"GPT (GUID partition table)","prefix":"些操作系统无法存取。因此后来又多了一个新的磁盘分区格式，称为  ","suffix":"！  这两种分区格式与限制不太相同啦！ 那么分区表又是啥？其实妳"}]}]}
>```
>%%
>*%%PREFIX%%些操作系统无法存取。因此后来又多了一个新的磁盘分区格式，称为%%HIGHLIGHT%% ==GPT (GUID partition table)== %%POSTFIX%%！  这两种分区格式与限制不太相同啦！ 那么分区表又是啥？其实妳*
>%%LINK%%[[#^6t900n34c25|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#硬盘
^6t900n34c25


>%%
>```annotation-json
>{"created":"2023-12-05T11:19:16.438Z","text":"如果为了分更多的分区，你就一定得留出一个延伸分区。","updated":"2023-12-05T11:19:16.438Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":105822,"end":105845},{"type":"TextQuoteSelector","exact":"主要分区与延伸分区最多可以有四笔(硬盘的限制)","prefix":" 主要分区、延伸分区与逻辑分区的特性我们作个简单的定义啰：  ","suffix":"  延伸分区最多只能有一个(操作系统的限制)  逻辑分区是由"}]}]}
>```
>%%
>*%%PREFIX%%主要分区、延伸分区与逻辑分区的特性我们作个简单的定义啰： %%HIGHLIGHT%% ==主要分区与延伸分区最多可以有四笔(硬盘的限制)== %%POSTFIX%% 延伸分区最多只能有一个(操作系统的限制)  逻辑分区是由*
>%%LINK%%[[#^230g9vylf9ph|show annotation]]
>%%COMMENT%%
>如果为了分更多的分区，你就一定得留出一个延伸分区。
>%%TAGS%%
>#硬盘
^230g9vylf9ph


>%%
>```annotation-json
>{"created":"2023-12-05T11:20:00.019Z","text":"延伸分区是将这么多逻辑分区统称起来的名字。\n所以说真正起作用的是逻辑分区而不是延伸分区，毕竟延伸分区严格来说只是一个名字罢了。","updated":"2023-12-05T11:20:00.019Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":105871,"end":105891},{"type":"TextQuoteSelector","exact":"逻辑分区是由延伸分区持续切割出来的分区槽","prefix":"硬盘的限制)  延伸分区最多只能有一个(操作系统的限制)  ","suffix":"；  能够被格式化后，作为数据存取的分区槽为主要分区与逻辑分区"}]}]}
>```
>%%
>*%%PREFIX%%硬盘的限制)  延伸分区最多只能有一个(操作系统的限制) %%HIGHLIGHT%% ==逻辑分区是由延伸分区持续切割出来的分区槽== %%POSTFIX%%；  能够被格式化后，作为数据存取的分区槽为主要分区与逻辑分区*
>%%LINK%%[[#^y8byey20qdp|show annotation]]
>%%COMMENT%%
>延伸分区是将这么多逻辑分区统称起来的名字。
>所以说真正起作用的是逻辑分区而不是延伸分区，毕竟延伸分区严格来说只是一个名字罢了。
>%%TAGS%%
>#硬盘
^y8byey20qdp


>%%
>```annotation-json
>{"created":"2023-12-05T11:21:19.728Z","text":"尽管延伸分区会有 /dev/sda4 这样的文件名，但是事实上文件都不存在这个目录下，而是会存在 /dev/sda5 等等逻辑分区当中。","updated":"2023-12-05T11:21:19.728Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":107513,"end":107530},{"type":"TextQuoteSelector","exact":"1~4 号是保留给主要/延伸分区槽","prefix":"E 的环境：   图 2.2.6、分区示意图 注意到了吗？因为 ","suffix":"的，因此第一个逻辑分区槽一定是由 5 号开始的！再次强调啊！  "}]}]}
>```
>%%
>*%%PREFIX%%E 的环境：   图 2.2.6、分区示意图 注意到了吗？因为%%HIGHLIGHT%% ==1~4 号是保留给主要/延伸分区槽== %%POSTFIX%%的，因此第一个逻辑分区槽一定是由 5 号开始的！再次强调啊！*
>%%LINK%%[[#^xeciatqml1l|show annotation]]
>%%COMMENT%%
>尽管延伸分区会有 /dev/sda4 这样的文件名，但是事实上文件都不存在这个目录下，而是会存在 /dev/sda5 等等逻辑分区当中。
>%%TAGS%%
>#硬盘
^xeciatqml1l


>%%
>```annotation-json
>{"created":"2023-12-11T06:18:53.642Z","text":"高级格式化又称逻辑格式化，它是指根据用户选定的文件系统（如FAT12、FAT16、FAT32、NTFS、EXT2、EXT3等），在磁盘的特定区域写入特定数据，以达到初始化磁盘或磁盘分区、清除原磁盘或磁盘分区中所有文件的一个操作。高级格式化包括对主引导记录中分区表相应区域的重写、根据用户选定的文件系统，在分区中划出一片用于存放文件分配表、目录表等用于文件管理的磁盘空间，以便用户使用该分区管理文件。\n\n看了后面可能可以清楚一点。例如llinux需要分出 inode 和 block 分区。","updated":"2023-12-11T06:18:53.642Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":307818,"end":307904},{"type":"TextQuoteSelector","exact":"每种操作系统所设定的文件属性/权限并不相同，  为了存放这些文件所需的数据，因此就需要将分区槽进行格式化，以成为操作系统能够利用的『文件系统格式(filesystem)』。","prefix":"才能够使用这个文件系统。  为什么需要进行『格式化』呢？这是因为","suffix":" 由此我们也能够知道，每种操作系统能够使用的文件系统并不相同。 "}]}]}
>```
>%%
>*%%PREFIX%%才能够使用这个文件系统。  为什么需要进行『格式化』呢？这是因为%%HIGHLIGHT%% ==每种操作系统所设定的文件属性/权限并不相同，  为了存放这些文件所需的数据，因此就需要将分区槽进行格式化，以成为操作系统能够利用的『文件系统格式(filesystem)』。== %%POSTFIX%%由此我们也能够知道，每种操作系统能够使用的文件系统并不相同。*
>%%LINK%%[[#^3wvxr2wow2a|show annotation]]
>%%COMMENT%%
>高级格式化又称逻辑格式化，它是指根据用户选定的文件系统（如FAT12、FAT16、FAT32、NTFS、EXT2、EXT3等），在磁盘的特定区域写入特定数据，以达到初始化磁盘或磁盘分区、清除原磁盘或磁盘分区中所有文件的一个操作。高级格式化包括对主引导记录中分区表相应区域的重写、根据用户选定的文件系统，在分区中划出一片用于存放文件分配表、目录表等用于文件管理的磁盘空间，以便用户使用该分区管理文件。
>
>看了后面可能可以清楚一点。例如llinux需要分出 inode 和 block 分区。
>%%TAGS%%
>#硬盘, #分区
^3wvxr2wow2a


>%%
>```annotation-json
>{"created":"2023-12-11T06:21:40.711Z","updated":"2023-12-11T06:21:40.711Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":307915,"end":307934},{"type":"TextQuoteSelector","exact":"每种操作系统能够使用的文件系统并不相同","prefix":"『文件系统格式(filesystem)』。 由此我们也能够知道，","suffix":"。  举例来说，windows 98  以前的微软操作系统主要利"}]}]}
>```
>%%
>*%%PREFIX%%『文件系统格式(filesystem)』。 由此我们也能够知道，%%HIGHLIGHT%% ==每种操作系统能够使用的文件系统并不相同== %%POSTFIX%%。  举例来说，windows 98  以前的微软操作系统主要利*
>%%LINK%%[[#^qslljsat87h|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^qslljsat87h


>%%
>```annotation-json
>{"created":"2023-12-11T06:23:16.049Z","updated":"2023-12-11T06:23:16.049Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":308448,"end":308519},{"type":"TextQuoteSelector","exact":"文件数据除了文件实际内容外，  通常含有非常多的属性，例如  Linux  操作系统的文件权限(rwx)与文件属性(拥有者、群组、时间参数等)","prefix":"系统是如何运作的呢？这与操作系统的文件数据有关。较新的操作系统的","suffix":"。 文件系统通常会将这两部份的数据分别存放在不同的区块，权限与属"}]}]}
>```
>%%
>*%%PREFIX%%系统是如何运作的呢？这与操作系统的文件数据有关。较新的操作系统的%%HIGHLIGHT%% ==文件数据除了文件实际内容外，  通常含有非常多的属性，例如  Linux  操作系统的文件权限(rwx)与文件属性(拥有者、群组、时间参数等)== %%POSTFIX%%。 文件系统通常会将这两部份的数据分别存放在不同的区块，权限与属*
>%%LINK%%[[#^sz1r1ff6cnp|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^sz1r1ff6cnp


>%%
>```annotation-json
>{"created":"2023-12-11T06:23:34.914Z","text":"文件系统这个概念还是十分的抽象","updated":"2023-12-11T06:23:34.914Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":308521,"end":308670},{"type":"TextQuoteSelector","exact":"文件系统通常会将这两部份的数据分别存放在不同的区块，权限与属性放置到 inode  中，至于实际数据则放置到  data block  区块中。  另外，还有一个超级区块  (superblock)  会记录整个文件系统的整体信息，包括  inode  与  block  的总量、使用量、剩余量等","prefix":"统的文件权限(rwx)与文件属性(拥有者、群组、时间参数等)。 ","suffix":"。 每个  inode  与  block  都有编号，至于这三"}]}]}
>```
>%%
>*%%PREFIX%%统的文件权限(rwx)与文件属性(拥有者、群组、时间参数等)。%%HIGHLIGHT%% ==文件系统通常会将这两部份的数据分别存放在不同的区块，权限与属性放置到 inode  中，至于实际数据则放置到  data block  区块中。  另外，还有一个超级区块  (superblock)  会记录整个文件系统的整体信息，包括  inode  与  block  的总量、使用量、剩余量等== %%POSTFIX%%。 每个  inode  与  block  都有编号，至于这三*
>%%LINK%%[[#^bqrwt5t8rnf|show annotation]]
>%%COMMENT%%
>文件系统这个概念还是十分的抽象
>%%TAGS%%
>#文件系统
^bqrwt5t8rnf


>%%
>```annotation-json
>{"created":"2023-12-11T06:24:17.645Z","updated":"2023-12-11T06:24:17.645Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":308816,"end":308830},{"type":"TextQuoteSelector","exact":"一个文件占用一个 inode","prefix":"及文件系统的格式与相关信息等；  inode：记录文件的属性，","suffix":"，同时记录此文件的数据所在的  block  号码；  blo"}]}]}
>```
>%%
>*%%PREFIX%%及文件系统的格式与相关信息等；  inode：记录文件的属性，%%HIGHLIGHT%% ==一个文件占用一个 inode== %%POSTFIX%%，同时记录此文件的数据所在的  block  号码；  blo*
>%%LINK%%[[#^bujh9tay1gv|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^bujh9tay1gv


>%%
>```annotation-json
>{"created":"2023-12-11T06:24:25.742Z","updated":"2023-12-11T06:24:25.742Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":308876,"end":308894},{"type":"TextQuoteSelector","exact":"文件太大时，会占用多个  block","prefix":"  block  号码；  block：实际记录文件的内容，若","suffix":"  。 由于每个  inode  与  block  都有编号，"}]}]}
>```
>%%
>*%%PREFIX%%block  号码；  block：实际记录文件的内容，若%%HIGHLIGHT%% ==文件太大时，会占用多个  block== %%POSTFIX%%。 由于每个  inode  与  block  都有编号，*
>%%LINK%%[[#^gmtr38dtug|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^gmtr38dtug


>%%
>```annotation-json
>{"created":"2023-12-11T06:24:53.355Z","text":"是因为搜索 inode 比搜索 block 更快吗？\n","updated":"2023-12-11T06:24:53.355Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":309103,"end":309111},{"type":"TextQuoteSelector","exact":"读写的效能比较好","prefix":"法，因为如此一来我们的磁盘就能够在短时间内读取出全部的数据，  ","suffix":"啰。 我们将  inode  与  block  区块用图解来说"}]}]}
>```
>%%
>*%%PREFIX%%法，因为如此一来我们的磁盘就能够在短时间内读取出全部的数据，%%HIGHLIGHT%% ==读写的效能比较好== %%POSTFIX%%啰。 我们将  inode  与  block  区块用图解来说*
>%%LINK%%[[#^kohii424v3c|show annotation]]
>%%COMMENT%%
>是因为搜索 inode 比搜索 block 更快吗？
>
>%%TAGS%%
>#文件系统
^kohii424v3c


>%%
>```annotation-json
>{"created":"2023-12-11T06:25:55.195Z","updated":"2023-12-11T06:25:55.195Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":309400,"end":309427},{"type":"TextQuoteSelector","exact":"索引式文件系统(indexed allocation)","prefix":"ode/block  资料存取示意图 这种数据存取的方法我们称为","suffix":"。那有没有其他的惯用文件系统可以比较一下啊？  有的，那就是我们"}]}]}
>```
>%%
>*%%PREFIX%%ode/block  资料存取示意图 这种数据存取的方法我们称为%%HIGHLIGHT%% ==索引式文件系统(indexed allocation)== %%POSTFIX%%。那有没有其他的惯用文件系统可以比较一下啊？  有的，那就是我们*
>%%LINK%%[[#^na1ovr1l8b|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^na1ovr1l8b


>%%
>```annotation-json
>{"created":"2023-12-11T06:26:28.862Z","text":"形成一个链表","updated":"2023-12-11T06:26:28.862Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":309525,"end":309593},{"type":"TextQuoteSelector","exact":" FAT  没有办法将这个文件的所有  block  在一开始就读取出来。每个  block  号码都记录在前一个  block  当中","prefix":"FAT  这种格式的文件系统并没有  inode  存在，所以 ","suffix":"，  他的读取方式有点像底下这样：  图 7.1.2、FAT 文"}]}]}
>```
>%%
>*%%PREFIX%%FAT  这种格式的文件系统并没有  inode  存在，所以%%HIGHLIGHT%% ==FAT  没有办法将这个文件的所有  block  在一开始就读取出来。每个  block  号码都记录在前一个  block  当中== %%POSTFIX%%，  他的读取方式有点像底下这样：  图 7.1.2、FAT 文*
>%%LINK%%[[#^sizlgybv0tt|show annotation]]
>%%COMMENT%%
>形成一个链表
>%%TAGS%%
>#文件系统
^sizlgybv0tt


>%%
>```annotation-json
>{"created":"2023-12-11T06:27:02.408Z","text":"原来这就是读写效能低的意思啊","updated":"2023-12-11T06:27:02.408Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":309825,"end":309830},{"type":"TextQuoteSelector","exact":"多转好几圈","prefix":"的磁盘读取头将无法在磁盘转一圈就读到所有的数据，  因此磁盘就会","suffix":"才能完整的读取到这个文件的内容！ 常常会听到所谓的『碎片整理』吧"}]}]}
>```
>%%
>*%%PREFIX%%的磁盘读取头将无法在磁盘转一圈就读到所有的数据，  因此磁盘就会%%HIGHLIGHT%% ==多转好几圈== %%POSTFIX%%才能完整的读取到这个文件的内容！ 常常会听到所谓的『碎片整理』吧*
>%%LINK%%[[#^m4jmz84gn8c|show annotation]]
>%%COMMENT%%
>原来这就是读写效能低的意思啊
>%%TAGS%%
>#文件系统
^m4jmz84gn8c


>%%
>```annotation-json
>{"created":"2023-12-11T06:27:36.061Z","updated":"2023-12-11T06:27:36.061Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":309856,"end":309860},{"type":"TextQuoteSelector","exact":"碎片整理","prefix":"会多转好几圈才能完整的读取到这个文件的内容！ 常常会听到所谓的『","suffix":"』吧？ 需要碎片整理的原因就是文件写入的  block  太过于"}]}]}
>```
>%%
>*%%PREFIX%%会多转好几圈才能完整的读取到这个文件的内容！ 常常会听到所谓的『%%HIGHLIGHT%% ==碎片整理== %%POSTFIX%%』吧？ 需要碎片整理的原因就是文件写入的  block  太过于*
>%%LINK%%[[#^31nntousdai|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^31nntousdai


>%%
>```annotation-json
>{"created":"2023-12-11T06:27:46.406Z","updated":"2023-12-11T06:27:46.406Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":309921,"end":309964},{"type":"TextQuoteSelector","exact":"透过碎片整理将同一个文件所属的  blocks  汇整在一起，这样数据的读取会比较容易","prefix":"太过于离散了，此时文件读取的效能将会变的很差所致。 这个时候可以","suffix":"啊！ 想当然尔，FAT  的文件系统需要经常的碎片整理一下，那么"}]}]}
>```
>%%
>*%%PREFIX%%太过于离散了，此时文件读取的效能将会变的很差所致。 这个时候可以%%HIGHLIGHT%% ==透过碎片整理将同一个文件所属的  blocks  汇整在一起，这样数据的读取会比较容易== %%POSTFIX%%啊！ 想当然尔，FAT  的文件系统需要经常的碎片整理一下，那么*
>%%LINK%%[[#^qvfq96htubo|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^qvfq96htubo


>%%
>```annotation-json
>{"created":"2023-12-11T06:31:39.309Z","updated":"2023-12-11T06:31:39.309Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":310728,"end":310739},{"type":"TextQuoteSelector","exact":"block group","prefix":"xt2  文件系统在格式化的时候基本上是区分为多个区块群组  (","suffix":")  的，每个区块群组都有独立的  inode/block/su"}]}]}
>```
>%%
>*%%PREFIX%%xt2  文件系统在格式化的时候基本上是区分为多个区块群组  (%%HIGHLIGHT%% ==block group== %%POSTFIX%%)  的，每个区块群组都有独立的  inode/block/su*
>%%LINK%%[[#^psr5b4mqzu9|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^psr5b4mqzu9


>%%
>```annotation-json
>{"created":"2023-12-11T06:32:41.150Z","updated":"2023-12-11T06:32:41.150Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":311279,"end":311298},{"type":"TextQuoteSelector","exact":"最大磁盘容量与最大单一文件容量并不相同","prefix":"是，由于  block  大小的差异，会导致该文件系统能够支持的","suffix":"。  因为  block  大小而产生的  Ext2  文件系统"}]}]}
>```
>%%
>*%%PREFIX%%是，由于  block  大小的差异，会导致该文件系统能够支持的%%HIGHLIGHT%% ==最大磁盘容量与最大单一文件容量并不相同== %%POSTFIX%%。  因为  block  大小而产生的  Ext2  文件系统*
>%%LINK%%[[#^engu259mhun|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^engu259mhun


>%%
>```annotation-json
>{"created":"2023-12-11T06:33:35.047Z","updated":"2023-12-11T06:33:35.047Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":311868,"end":311923},{"type":"TextQuoteSelector","exact":"如果你的文件都非常小，但是你的  block  在格式化时却选用最大的  4K  时，可能会产生一些容量的浪费","prefix":"所说，由于每个  block  仅能容纳一个文件的数据而已，因此","suffix":"喔！我们以底下的一个简单例题来算一下空间的浪费吧！ 例题： 假设"}]}]}
>```
>%%
>*%%PREFIX%%所说，由于每个  block  仅能容纳一个文件的数据而已，因此%%HIGHLIGHT%% ==如果你的文件都非常小，但是你的  block  在格式化时却选用最大的  4K  时，可能会产生一些容量的浪费== %%POSTFIX%%喔！我们以底下的一个简单例题来算一下空间的浪费吧！ 例题： 假设*
>%%LINK%%[[#^3l1hz8ehp5m|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^3l1hz8ehp5m


>%%
>```annotation-json
>{"created":"2023-12-11T06:34:09.375Z","text":"一个文件被分到越多不同的 block ，读写效能就越差","updated":"2023-12-11T06:34:09.375Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":312457,"end":312542},{"type":"TextQuoteSelector","exact":"block  较小的话，那么大型文件将会占用数量更多的  block  ，而   inode  也要记录更多的  block  号码，此时将可能导致文件系统不良的读写效能","prefix":"lock  大小订为  1K  即可？  这也不妥，因为如果  ","suffix":"。 所以我们可以说，在您进行文件系统的格式化之前，请先想好该文件"}]}]}
>```
>%%
>*%%PREFIX%%lock  大小订为  1K  即可？  这也不妥，因为如果%%HIGHLIGHT%% ==block  较小的话，那么大型文件将会占用数量更多的  block  ，而   inode  也要记录更多的  block  号码，此时将可能导致文件系统不良的读写效能== %%POSTFIX%%。 所以我们可以说，在您进行文件系统的格式化之前，请先想好该文件*
>%%LINK%%[[#^feghcv7dj6|show annotation]]
>%%COMMENT%%
>一个文件被分到越多不同的 block ，读写效能就越差
>%%TAGS%%
>#文件系统
^feghcv7dj6


>%%
>```annotation-json
>{"created":"2023-12-11T06:35:13.157Z","text":"根据自己需求来，没有绝对的好坏","updated":"2023-12-11T06:35:13.157Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":312569,"end":312583},{"type":"TextQuoteSelector","exact":"想好该文件系统预计使用的情况","prefix":"的读写效能。 所以我们可以说，在您进行文件系统的格式化之前，请先","suffix":"。  以鸟哥来说，我的数值模式仿真平台随便一个文件都好几百  M"}]}]}
>```
>%%
>*%%PREFIX%%的读写效能。 所以我们可以说，在您进行文件系统的格式化之前，请先%%HIGHLIGHT%% ==想好该文件系统预计使用的情况== %%POSTFIX%%。  以鸟哥来说，我的数值模式仿真平台随便一个文件都好几百  M*
>%%LINK%%[[#^nbyhynie9o|show annotation]]
>%%COMMENT%%
>根据自己需求来，没有绝对的好坏
>%%TAGS%%
>#文件系统
^nbyhynie9o


>%%
>```annotation-json
>{"created":"2023-12-11T06:37:56.817Z","text":"如果 inode 放不下 block 的记录了，那么这个文件也就不能再占用更多的空间了","updated":"2023-12-11T06:37:56.817Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":313054,"end":313079},{"type":"TextQuoteSelector","exact":"inode  的数量与大小也是在格式化时就已经固定","prefix":"ID...；  该文件真正内容的指向  (pointer)； ","suffix":"了，除此之外  inode  还有些什么特色呢？  每个  i"}]}]}
>```
>%%
>*%%PREFIX%%ID...；  该文件真正内容的指向  (pointer)；%%HIGHLIGHT%% ==inode  的数量与大小也是在格式化时就已经固定== %%POSTFIX%%了，除此之外  inode  还有些什么特色呢？  每个  i*
>%%LINK%%[[#^34gmq7usvat|show annotation]]
>%%COMMENT%%
>如果 inode 放不下 block 的记录了，那么这个文件也就不能再占用更多的空间了
>%%TAGS%%
>
^34gmq7usvat


>%%
>```annotation-json
>{"created":"2023-12-11T06:41:58.250Z","text":"所以一个文件系统是 inode block superblock 的集合？","updated":"2023-12-11T06:41:58.250Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":314911,"end":314948},{"type":"TextQuoteSelector","exact":"没有  Superblock  ，就没有这个  filesystem  了","prefix":"k  是记录整个  filesystem  相关信息的地方，  ","suffix":"。他记录的信息主要有：  block  与  inode  的"}]}]}
>```
>%%
>*%%PREFIX%%k  是记录整个  filesystem  相关信息的地方，%%HIGHLIGHT%% ==没有  Superblock  ，就没有这个  filesystem  了== %%POSTFIX%%。他记录的信息主要有：  block  与  inode  的*
>%%LINK%%[[#^t6doo4oxnja|show annotation]]
>%%COMMENT%%
>所以一个文件系统是 inode block superblock 的集合？
>%%TAGS%%
>#文件系统
^t6doo4oxnja


>%%
>```annotation-json
>{"created":"2023-12-11T06:44:26.450Z","updated":"2023-12-11T06:44:26.450Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":315578,"end":315652},{"type":"TextQuoteSelector","exact":"若含有  superblock  则该  superblock  主要是做为第一个  block group  内  superblock  的备份","prefix":"k group  不一定含有  superblock  ，  而","suffix":"咯，这样可以进行  superblock  的救援呢！  Fi"}]}]}
>```
>%%
>*%%PREFIX%%k group  不一定含有  superblock  ，  而%%HIGHLIGHT%% ==若含有  superblock  则该  superblock  主要是做为第一个  block group  内  superblock  的备份== %%POSTFIX%%咯，这样可以进行  superblock  的救援呢！  Fi*
>%%LINK%%[[#^rrae6n0de6h|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#文件系统
^rrae6n0de6h


>%%
>```annotation-json
>{"created":"2023-12-11T06:44:28.792Z","text":"但是可以有备份\n","updated":"2023-12-11T06:44:28.792Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":315455,"end":315467},{"type":"TextQuoteSelector","exact":"一个文件系统应该仅有一个","prefix":"oup  都可能含有  superblock  喔！但是我们也说","suffix":" superblock  而已，那是怎么回事啊？  事实上除了第"}]}]}
>```
>%%
>*%%PREFIX%%oup  都可能含有  superblock  喔！但是我们也说%%HIGHLIGHT%% ==一个文件系统应该仅有一个== %%POSTFIX%%superblock  而已，那是怎么回事啊？  事实上除了第*
>%%LINK%%[[#^dhq9tvke6p8|show annotation]]
>%%COMMENT%%
>但是可以有备份
>
>%%TAGS%%
>#文件系统
^dhq9tvke6p8


>%%
>```annotation-json
>{"created":"2023-12-11T10:44:14.102Z","text":"ext filesystem专用","updated":"2023-12-11T10:44:14.102Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":316335,"end":316343},{"type":"TextQuoteSelector","exact":"dumpe2fs","prefix":"map  则是记录使用与未使用的  inode  号码啰！  ","suffix":"：  查询  Ext  家族  superblock  信息的指"}]}]}
>```
>%%
>*%%PREFIX%%map  则是记录使用与未使用的  inode  号码啰！ %%HIGHLIGHT%% ==dumpe2fs== %%POSTFIX%%：  查询  Ext  家族  superblock  信息的指*
>%%LINK%%[[#^rwgrio1t3xk|show annotation]]
>%%COMMENT%%
>ext filesystem专用
>%%TAGS%%
>#文件系统
^rwgrio1t3xk


>%%
>```annotation-json
>{"created":"2023-12-11T10:44:42.126Z","text":"block id\n","updated":"2023-12-11T10:44:42.126Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":316822,"end":316827},{"type":"TextQuoteSelector","exact":"blkid","prefix":"1GB ext4 文件系统内容 [root@study ~]# ","suffix":"   <==这个指令可以叫出目前系统有被格式化的装置 /dev/"}]}]}
>```
>%%
>*%%PREFIX%%1GB ext4 文件系统内容 [root@study ~]#%%HIGHLIGHT%% ==blkid== %%POSTFIX%%<==这个指令可以叫出目前系统有被格式化的装置 /dev/*
>%%LINK%%[[#^vy3emkp5p9|show annotation]]
>%%COMMENT%%
>block id
>
>%%TAGS%%
>#文件系统
^vy3emkp5p9


>%%
>```annotation-json
>{"created":"2023-12-11T10:47:29.119Z","text":"inode 着实有点像这个文件的指针，通过它可以找到这个文件的实际内容。","updated":"2023-12-11T10:47:29.119Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":320913,"end":320958},{"type":"TextQuoteSelector","exact":"而  block  则是记录在这个目录下的文件名与该文件名占用的  inode  号码数据","prefix":"相关权限与属性，并可记录分配到的那块  block  号码；  ","suffix":"。也就是说目录所占用的  block  内容在记录如下的信息： "}]}]}
>```
>%%
>*%%PREFIX%%相关权限与属性，并可记录分配到的那块  block  号码；%%HIGHLIGHT%% ==而  block  则是记录在这个目录下的文件名与该文件名占用的  inode  号码数据== %%POSTFIX%%。也就是说目录所占用的  block  内容在记录如下的信息：*
>%%LINK%%[[#^87kt5mw8nhc|show annotation]]
>%%COMMENT%%
>inode 着实有点像这个文件的指针，通过它可以找到这个文件的实际内容。
>%%TAGS%%
>#文件系统
^87kt5mw8nhc


>%%
>```annotation-json
>{"created":"2023-12-11T10:50:07.299Z","text":"这里就可以统一目录与文件了。目录 block 内的实际内容就是文件名与 inode的对照。","updated":"2023-12-11T10:50:07.299Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":322106,"end":322177},{"type":"TextQuoteSelector","exact":"一个  block  无法容纳的下所有的档名与  inode  对照表时，Linux  会给予该目录多一个  block 来继续记录相关的数据","prefix":"lock  而已，也就是说：  在目录底下的文件数如果太多而导致","suffix":"；  文件： 当我们在  Linux  下的  ext2  建"}]}]}
>```
>%%
>*%%PREFIX%%lock  而已，也就是说：  在目录底下的文件数如果太多而导致%%HIGHLIGHT%% ==一个  block  无法容纳的下所有的档名与  inode  对照表时，Linux  会给予该目录多一个  block 来继续记录相关的数据== %%POSTFIX%%；  文件： 当我们在  Linux  下的  ext2  建*
>%%LINK%%[[#^v9udnsgwurj|show annotation]]
>%%COMMENT%%
>这里就可以统一目录与文件了。目录 block 内的实际内容就是文件名与 inode的对照。
>%%TAGS%%
>#文件系统
^v9udnsgwurj


>%%
>```annotation-json
>{"created":"2023-12-11T10:51:36.031Z","updated":"2023-12-11T10:51:36.031Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":322466,"end":322505},{"type":"TextQuoteSelector","exact":"inode  本身并不记录文件名，文件名的记录是在目录的  block  当中","prefix":" 目录树读取： 好了，经过上面的说明你也应该要很清楚的知道  ","suffix":"。  因此在第五章文件与目录的权限说明中，  我们才会提到『新增"}]}]}
>```
>%%
>*%%PREFIX%% 目录树读取： 好了，经过上面的说明你也应该要很清楚的知道%%HIGHLIGHT%% ==inode  本身并不记录文件名，文件名的记录是在目录的  block  当中== %%POSTFIX%%。  因此在第五章文件与目录的权限说明中，  我们才会提到『新增*
>%%LINK%%[[#^p841k09zljd|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^p841k09zljd


>%%
>```annotation-json
>{"created":"2023-12-11T10:53:28.767Z","text":"inode 是 block 的守门人","updated":"2023-12-11T10:53:28.767Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":323215,"end":323258},{"type":"TextQuoteSelector","exact":"inode  规范的权限让我们可以读取该  block 的内容(有  r  与  x)","prefix":"inode  号码为  128  的根目录  inode，且  ","suffix":"  ； 2. /  的  block： 经过上个步骤取得  bl"}]}]}
>```
>%%
>*%%PREFIX%%inode  号码为  128  的根目录  inode，且%%HIGHLIGHT%% ==inode  规范的权限让我们可以读取该  block 的内容(有  r  与  x)== %%POSTFIX%%； 2. /  的  block： 经过上个步骤取得  bl*
>%%LINK%%[[#^o1bafnuic2|show annotation]]
>%%COMMENT%%
>inode 是 block 的守门人
>%%TAGS%%
>#文件系统
^o1bafnuic2


>%%
>```annotation-json
>{"created":"2023-12-11T10:55:27.680Z","updated":"2023-12-11T10:55:27.680Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":323956,"end":323983},{"type":"TextQuoteSelector","exact":"如果文件真的太过离散，确实还是会发生读取效率低落的问题","prefix":"  block  号码都记上了，  所以资料可以一次性读取，但是","suffix":"。  因为磁盘读取头还是得要在整个文件系统中来来去去的频繁读取！"}]}]}
>```
>%%
>*%%PREFIX%%block  号码都记上了，  所以资料可以一次性读取，但是%%HIGHLIGHT%% ==如果文件真的太过离散，确实还是会发生读取效率低落的问题== %%POSTFIX%%。  因为磁盘读取头还是得要在整个文件系统中来来去去的频繁读取！*
>%%LINK%%[[#^h9np4qkxsfg|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^h9np4qkxsfg


>%%
>```annotation-json
>{"created":"2023-12-11T10:56:11.772Z","text":"是不是因为复制是按文件顺序复制的。复制完一个文件才进行下一个文件的复制。所以经过一次复制，他就自动地帮你把 block 号重排一遍了。","updated":"2023-12-11T10:56:11.772Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":324049,"end":324053},{"type":"TextQuoteSelector","exact":"复制出来","prefix":"果真如此，那么可以将整个  filesystme  内的数据全部","suffix":"，将该  filesystem  重新格式化，  再将数据给他复"}]}]}
>```
>%%
>*%%PREFIX%%果真如此，那么可以将整个  filesystme  内的数据全部%%HIGHLIGHT%% ==复制出来== %%POSTFIX%%，将该  filesystem  重新格式化，  再将数据给他复*
>%%LINK%%[[#^irjv56a55n|show annotation]]
>%%COMMENT%%
>是不是因为复制是按文件顺序复制的。复制完一个文件才进行下一个文件的复制。所以经过一次复制，他就自动地帮你把 block 号重排一遍了。
>%%TAGS%%
>#文件系统
^irjv56a55n


>%%
>```annotation-json
>{"created":"2023-12-11T10:57:56.230Z","updated":"2023-12-11T10:57:56.230Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":316005,"end":316042},{"type":"TextQuoteSelector","exact":"从  block bitmap  当中可以知道哪些  block  是空的","prefix":" 是空的？这就得要透过  block bitmap  的辅助了。","suffix":"，因此我们的系统就能够很快速的找到可使用的空间来处置文件啰。 同"}]}]}
>```
>%%
>*%%PREFIX%%是空的？这就得要透过  block bitmap  的辅助了。%%HIGHLIGHT%% ==从  block bitmap  当中可以知道哪些  block  是空的== %%POSTFIX%%，因此我们的系统就能够很快速的找到可使用的空间来处置文件啰。 同*
>%%LINK%%[[#^8zpzdt87w0o|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^8zpzdt87w0o


>%%
>```annotation-json
>{"created":"2023-12-11T10:58:07.261Z","updated":"2023-12-11T10:58:07.261Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":316294,"end":316330},{"type":"TextQuoteSelector","exact":"inode bitmap  则是记录使用与未使用的  inode  号码","prefix":"ap  记录的是使用与未使用的  block  号码， 至于  ","suffix":"啰！  dumpe2fs：  查询  Ext  家族  sup"}]}]}
>```
>%%
>*%%PREFIX%%ap  记录的是使用与未使用的  block  号码， 至于%%HIGHLIGHT%% ==inode bitmap  则是记录使用与未使用的  inode  号码== %%POSTFIX%%啰！  dumpe2fs：  查询  Ext  家族  sup*
>%%LINK%%[[#^ajb15pews7a|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ajb15pews7a


>%%
>```annotation-json
>{"created":"2023-12-11T10:58:40.245Z","text":"必须有 w 才能新增！！因为你要向目录的 block 中写入东西！！！","updated":"2023-12-11T10:58:40.245Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":324472,"end":324473},{"type":"TextQuoteSelector","exact":"w","prefix":"系统的行为是： 1. 先确定用户对于欲新增文件的目录是否具有  ","suffix":"  与  x  的权限，若有的话才能新增； 2. 根据  ino"}]}]}
>```
>%%
>*%%PREFIX%%系统的行为是： 1. 先确定用户对于欲新增文件的目录是否具有%%HIGHLIGHT%% ==w== %%POSTFIX%%与  x  的权限，若有的话才能新增； 2. 根据  ino*
>%%LINK%%[[#^m9l5hq0gh9|show annotation]]
>%%COMMENT%%
>必须有 w 才能新增！！因为你要向目录的 block 中写入东西！！！
>%%TAGS%%
>#文件系统
^m9l5hq0gh9


>%%
>```annotation-json
>{"created":"2023-12-11T10:59:58.441Z","text":"真正的数据是存放在这里的。\n这里的数据较为稳定，与metadata形成对比。","updated":"2023-12-11T10:59:58.441Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":324736,"end":324772},{"type":"TextQuoteSelector","exact":"inode table  与  data block  称为数据存放区域","prefix":"并更新  superblock  的内容。 一般来说，我们将  ","suffix":"，至于其他例如  superblock、  block bitm"}]}]}
>```
>%%
>*%%PREFIX%%并更新  superblock  的内容。 一般来说，我们将%%HIGHLIGHT%% ==inode table  与  data block  称为数据存放区域== %%POSTFIX%%，至于其他例如  superblock、  block bitm*
>%%LINK%%[[#^gs2r58ntd9j|show annotation]]
>%%COMMENT%%
>真正的数据是存放在这里的。
>这里的数据较为稳定，与metadata形成对比。
>%%TAGS%%
>#文件系统
^gs2r58ntd9j


>%%
>```annotation-json
>{"created":"2023-12-11T11:03:01.303Z","text":"metadata","updated":"2023-12-11T11:03:01.303Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":324856,"end":324945},{"type":"TextQuoteSelector","exact":"superblock, inode bitmap  及 block bitmap  的数据是经常变动的，每次新增、移除、编辑时都可能会影响到这三个部分的数据，因此才被称为中介数据","prefix":" 等区段就被称为  metadata (中介资料)  啰，因为 ","suffix":"的啦。  数据的不一致  (Inconsistent)  状态"}]}]}
>```
>%%
>*%%PREFIX%%等区段就被称为  metadata (中介资料)  啰，因为%%HIGHLIGHT%% ==superblock, inode bitmap  及 block bitmap  的数据是经常变动的，每次新增、移除、编辑时都可能会影响到这三个部分的数据，因此才被称为中介数据== %%POSTFIX%%的啦。  数据的不一致  (Inconsistent)  状态*
>%%LINK%%[[#^t8jstrq8ye9|show annotation]]
>%%COMMENT%%
>metadata
>%%TAGS%%
>#文件系统
^t8jstrq8ye9


>%%
>```annotation-json
>{"created":"2023-12-11T11:05:33.151Z","updated":"2023-12-11T11:05:33.151Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":325081,"end":325198},{"type":"TextQuoteSelector","exact":"写入的数据仅有  inode table  及  data block  而已，  最后一个同步更新中介数据的步骤并没有做完，此时就会发生  metadata  的内容与实际数据存放区产生不一致 (Inconsistent) 的情况了","prefix":"如突然的停电啊、  系统核心发生错误啊～等等的怪事发生时)，所以","suffix":"。 既然有不一致当然就得要克服！在早期的  Ext2  文件系统"}]}]}
>```
>%%
>*%%PREFIX%%如突然的停电啊、  系统核心发生错误啊～等等的怪事发生时)，所以%%HIGHLIGHT%% ==写入的数据仅有  inode table  及  data block  而已，  最后一个同步更新中介数据的步骤并没有做完，此时就会发生  metadata  的内容与实际数据存放区产生不一致 (Inconsistent) 的情况了== %%POSTFIX%%。 既然有不一致当然就得要克服！在早期的  Ext2  文件系统*
>%%LINK%%[[#^bpxbcgl5o|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#文件系统
^bpxbcgl5o


>%%
>```annotation-json
>{"created":"2023-12-11T11:07:38.022Z","text":"把每次文件的写入记录下来，从而在不一致情况出现的时候可以不用大海捞针。","updated":"2023-12-11T11:07:38.022Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":325579,"end":325586},{"type":"TextQuoteSelector","exact":"日志式文件系统","prefix":"拉长～真是麻烦～这也就造成后来所谓日志式文件系统的兴起了。  ","suffix":"  (Journaling filesystem) 为了避免上述"}]}]}
>```
>%%
>*%%PREFIX%%拉长～真是麻烦～这也就造成后来所谓日志式文件系统的兴起了。 %%HIGHLIGHT%% ==日志式文件系统== %%POSTFIX%%(Journaling filesystem) 为了避免上述*
>%%LINK%%[[#^ldyqbfvibn|show annotation]]
>%%COMMENT%%
>把每次文件的写入记录下来，从而在不一致情况出现的时候可以不用大海捞针。
>%%TAGS%%
>#文件系统
^ldyqbfvibn


>%%
>```annotation-json
>{"created":"2023-12-11T11:10:03.438Z","text":"定期将脏数据写回，而不是每次操作都写回。","updated":"2023-12-11T11:10:03.438Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":326724,"end":326728},{"type":"TextQuoteSelector","exact":"异步处理","prefix":"效率的问题，因此我们的  Linux  使用的方式是透过一个称为","suffix":"  (asynchronously) 的方式。所谓的异步处理是这"}]}]}
>```
>%%
>*%%PREFIX%%效率的问题，因此我们的  Linux  使用的方式是透过一个称为%%HIGHLIGHT%% ==异步处理== %%POSTFIX%%(asynchronously) 的方式。所谓的异步处理是这*
>%%LINK%%[[#^mrectq66q3j|show annotation]]
>%%COMMENT%%
>定期将脏数据写回，而不是每次操作都写回。
>%%TAGS%%
>#文件系统
^mrectq66q3j


>%%
>```annotation-json
>{"created":"2023-12-11T11:11:08.924Z","updated":"2023-12-11T11:11:08.924Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":327132,"end":327151},{"type":"TextQuoteSelector","exact":"Linux  的物理内存最后都会被用光","prefix":"到主存储器的缓冲区，以加速文件系统的读/写；  承上，因此  ","suffix":"！这是正常的情况！可加速系统效能；  你可以手动使用  syn"}]}]}
>```
>%%
>*%%PREFIX%%到主存储器的缓冲区，以加速文件系统的读/写；  承上，因此%%HIGHLIGHT%% ==Linux  的物理内存最后都会被用光== %%POSTFIX%%！这是正常的情况！可加速系统效能；  你可以手动使用  syn*
>%%LINK%%[[#^eyolt3j8yd|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^eyolt3j8yd


>%%
>```annotation-json
>{"created":"2023-12-11T11:11:45.632Z","updated":"2023-12-11T11:11:45.632Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":327258,"end":327332},{"type":"TextQuoteSelector","exact":"但若不正常关机(如跳电、当机或其他不明原因)，由于数据尚未回写到磁盘内，  因此重新启动后可能会花很多时间在进行磁盘检验，甚至可能导致文件系统的损毁","prefix":"指令会主动呼叫  sync  来将内存的数据回写入磁盘内；  ","suffix":"(非磁盘损毁)。 7.1.7  挂载点的意义  (mount p"}]}]}
>```
>%%
>*%%PREFIX%%指令会主动呼叫  sync  来将内存的数据回写入磁盘内； %%HIGHLIGHT%% ==但若不正常关机(如跳电、当机或其他不明原因)，由于数据尚未回写到磁盘内，  因此重新启动后可能会花很多时间在进行磁盘检验，甚至可能导致文件系统的损毁== %%POSTFIX%%(非磁盘损毁)。 7.1.7  挂载点的意义  (mount p*
>%%LINK%%[[#^1cdo910odq7|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^1cdo910odq7


>%%
>```annotation-json
>{"created":"2023-12-11T11:11:52.050Z","text":"相当于一个传送门，进了他就相当于你进了一块磁盘上的物理空间。里面所有文件的 inode 信息都存储在这块物理空间内。\n\n是不是能理解为，要进入这个目录，就要先读取他的inode，而他的inode就在这块空间内，所以硬盘的机械臂就转到这块空间上了。\n\nlinux下面所有的文件、目录、设备都有一个路径°，这个路径永远以／开头，用／分隔，如果一个路径是另一个路径的前缀，则这两个路径有逻辑上的父子关系。但是并不是所有逻辑上的父子关系都必须要是同一个设备，决定不同路径对应到哪个设备的机制就叫做mount（挂载°)。通过mount，可以设置当前的路径与设备的对应关系。\n每个设备会设置一个挂载点°，挂载点是一个空目录。一般来说必须有一个设备挂载在／这个根路径下面，叫做rootfs°。其他挂载点可以是／tmp,/boot,/dev等等，通过在rootfs上面创建一个空目录然后用mount命令就可以将设备挂载到这个目录上。挂载之后，这个目录下的子路径°，就会映射到被挂载的设备里面。当访问一个路径时，会选择一个能最大匹配当前路径前缀的挂载点。比如说，有／var的挂载点，也有／var/run的挂载点的情况下，访问／var/run/test.pid°，就会匹配到／var/run挂载点设备下面的／test.pid。\n同一个设备可以有多个挂载点，同一个挂载点同时只能加载一个设备。访问非挂载点的路径的时候，按照前面所说，其实是访问最接近的一个挂载点，如果没有其他挂载点那么就是rootfs上的目录或者文件了。\n实际上并不只有linux支持挂载点，Windows也是一样支持的。去控制面板／管理工具／计算机管理°里面，挑一个磁盘（比如D盘），然后给它分一个新的挂载点试试，比如C:\\data","updated":"2023-12-11T11:11:52.050Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":327357,"end":327368},{"type":"TextQuoteSelector","exact":"mount point","prefix":"文件系统的损毁(非磁盘损毁)。 7.1.7  挂载点的意义  (","suffix":") 每个  filesystem  都有独立的  inode /"}]}]}
>```
>%%
>*%%PREFIX%%文件系统的损毁(非磁盘损毁)。 7.1.7  挂载点的意义  (%%HIGHLIGHT%% ==mount point== %%POSTFIX%%) 每个  filesystem  都有独立的  inode /*
>%%LINK%%[[#^iswxn8onvs|show annotation]]
>%%COMMENT%%
>相当于一个传送门，进了他就相当于你进了一块磁盘上的物理空间。里面所有文件的 inode 信息都存储在这块物理空间内。
>
>是不是能理解为，要进入这个目录，就要先读取他的inode，而他的inode就在这块空间内，所以硬盘的机械臂就转到这块空间上了。
>
>linux下面所有的文件、目录、设备都有一个路径°，这个路径永远以／开头，用／分隔，如果一个路径是另一个路径的前缀，则这两个路径有逻辑上的父子关系。但是并不是所有逻辑上的父子关系都必须要是同一个设备，决定不同路径对应到哪个设备的机制就叫做mount（挂载°)。通过mount，可以设置当前的路径与设备的对应关系。
>每个设备会设置一个挂载点°，挂载点是一个空目录。一般来说必须有一个设备挂载在／这个根路径下面，叫做rootfs°。其他挂载点可以是／tmp,/boot,/dev等等，通过在rootfs上面创建一个空目录然后用mount命令就可以将设备挂载到这个目录上。挂载之后，这个目录下的子路径°，就会映射到被挂载的设备里面。当访问一个路径时，会选择一个能最大匹配当前路径前缀的挂载点。比如说，有／var的挂载点，也有／var/run的挂载点的情况下，访问／var/run/test.pid°，就会匹配到／var/run挂载点设备下面的／test.pid。
>同一个设备可以有多个挂载点，同一个挂载点同时只能加载一个设备。访问非挂载点的路径的时候，按照前面所说，其实是访问最接近的一个挂载点，如果没有其他挂载点那么就是rootfs上的目录或者文件了。
>实际上并不只有linux支持挂载点，Windows也是一样支持的。去控制面板／管理工具／计算机管理°里面，挑一个磁盘（比如D盘），然后给它分一个新的挂载点试试，比如C:\data
>%%TAGS%%
>#文件系统
^iswxn8onvs


>%%
>```annotation-json
>{"created":"2023-12-11T11:13:36.070Z","updated":"2023-12-11T11:13:36.070Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":328203,"end":328234},{"type":"TextQuoteSelector","exact":"透过判断  inode  号码来确认不同文件名是否为相同的文件","prefix":"(因为一个文件占用一个  inode  之故)，  因此我们可以","suffix":"喔！所以可以这样看： [root@study ~]# ls -i"}]}]}
>```
>%%
>*%%PREFIX%%(因为一个文件占用一个  inode  之故)，  因此我们可以%%HIGHLIGHT%% ==透过判断  inode  号码来确认不同文件名是否为相同的文件== %%POSTFIX%%喔！所以可以这样看： [root@study ~]# ls -i*
>%%LINK%%[[#^g76qgkn24ub|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^g76qgkn24ub


>%%
>```annotation-json
>{"created":"2023-12-11T11:23:19.570Z","updated":"2023-12-11T11:23:19.570Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":329193,"end":329224},{"type":"TextQuoteSelector","exact":"VFS (Virtual Filesystem Switch)","prefix":"# cat /proc/filesystems  Linux ","suffix":" 了解了我们使用的文件系统之后，再来则是要提到，那么  Linu"}]}]}
>```
>%%
>*%%PREFIX%%# cat /proc/filesystems  Linux%%HIGHLIGHT%% ==VFS (Virtual Filesystem Switch)== %%POSTFIX%%了解了我们使用的文件系统之后，再来则是要提到，那么  Linu*
>%%LINK%%[[#^zo001qqjuen|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^zo001qqjuen


>%%
>```annotation-json
>{"created":"2023-12-11T11:33:35.400Z","updated":"2023-12-11T11:33:35.400Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":337595,"end":337615},{"type":"TextQuoteSelector","exact":"系统里面其实还有很多特殊的文件系统存在的","prefix":"   - /proc/sys/fs/binfmt_misc # ","suffix":"。那些比较特殊的文件系统几乎 # 都是在内存当中，例如 /pro"}]}]}
>```
>%%
>*%%PREFIX%%- /proc/sys/fs/binfmt_misc #%%HIGHLIGHT%% ==系统里面其实还有很多特殊的文件系统存在的== %%POSTFIX%%。那些比较特殊的文件系统几乎 # 都是在内存当中，例如 /pro*
>%%LINK%%[[#^er1lgvvtg7|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^er1lgvvtg7


>%%
>```annotation-json
>{"created":"2023-12-11T11:47:38.673Z","text":"在目录的 block 中，该文件名对应的 inode 号码与原本的文件名对应的 inode 号码相同。","updated":"2023-12-11T11:47:38.673Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":341512,"end":341559},{"type":"TextQuoteSelector","exact":"hard link  只是在某个目录下新增一笔档名链接到某  inode  号码的关连记录而已","prefix":"有的！那就是  hard link  的由来。  所以简单的说：","suffix":"。 举个例子来说，假设我系统有个  /root/crontab "}]}]}
>```
>%%
>*%%PREFIX%%有的！那就是  hard link  的由来。  所以简单的说：%%HIGHLIGHT%% ==hard link  只是在某个目录下新增一笔档名链接到某  inode  号码的关连记录而已== %%POSTFIX%%。 举个例子来说，假设我系统有个  /root/crontab*
>%%LINK%%[[#^kcqk5ncr1m|show annotation]]
>%%COMMENT%%
>在目录的 block 中，该文件名对应的 inode 号码与原本的文件名对应的 inode 号码相同。
>%%TAGS%%
>#文件系统
^kcqk5ncr1m


>%%
>```annotation-json
>{"created":"2023-12-11T11:50:40.466Z","updated":"2023-12-11T11:50:40.466Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":342116,"end":342160},{"type":"TextQuoteSelector","exact":"那个字段称为『连结』，这个字段的意义为：『有多少个档名链接到这个  inode  号码』","prefix":"！而且你也会发现第二个字段由原本的  1 变成  2  了！  ","suffix":"的意思。  如果将读取到正确数据的方式画成示意图，就类似如下画面"}]}]}
>```
>%%
>*%%PREFIX%%！而且你也会发现第二个字段由原本的  1 变成  2  了！%%HIGHLIGHT%% ==那个字段称为『连结』，这个字段的意义为：『有多少个档名链接到这个  inode  号码』== %%POSTFIX%%的意思。  如果将读取到正确数据的方式画成示意图，就类似如下画面*
>%%LINK%%[[#^2x4u1ll6utg|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^2x4u1ll6utg


>%%
>```annotation-json
>{"created":"2023-12-11T11:54:18.361Z","text":"为什么要给这个目录下的所有文件都添加 hard link？","updated":"2023-12-11T11:54:18.361Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":342957,"end":342969},{"type":"TextQuoteSelector","exact":"不能  link  目录","prefix":"nk  是有限制的：  不能跨  Filesystem；  ","suffix":"。 不能跨  Filesystem  还好理解，那不能  har"}]}]}
>```
>%%
>*%%PREFIX%%nk  是有限制的：  不能跨  Filesystem； %%HIGHLIGHT%% ==不能  link  目录== %%POSTFIX%%。 不能跨  Filesystem  还好理解，那不能  har*
>%%LINK%%[[#^pm7bzu0xnw|show annotation]]
>%%COMMENT%%
>为什么要给这个目录下的所有文件都添加 hard link？
>%%TAGS%%
>#文件系统
^pm7bzu0xnw


>%%
>```annotation-json
>{"created":"2023-12-11T11:59:56.722Z","text":"注意他是先去找目录的，并不是直接找到目标文件的 inode，否则就变成 hard link了。\n\n这个思想好像就是我在想的为什么要给目录底下的每个文件做 link，link到目录的 inode 不就好了嘛","updated":"2023-12-11T11:59:56.722Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":344108,"end":344131},{"type":"TextQuoteSelector","exact":"链接到正确的目录去取得目标文件的  inode","prefix":" 1  号  inode  读取到连结档的内容仅有档名，根据档名","suffix":"  ， 最终就能够读取到正确的数据了。你可以发现的是，如果目标文"}]}]}
>```
>%%
>*%%PREFIX%%1  号  inode  读取到连结档的内容仅有档名，根据档名%%HIGHLIGHT%% ==链接到正确的目录去取得目标文件的  inode== %%POSTFIX%%， 最终就能够读取到正确的数据了。你可以发现的是，如果目标文*
>%%LINK%%[[#^19mhzh3gyjb|show annotation]]
>%%COMMENT%%
>注意他是先去找目录的，并不是直接找到目标文件的 inode，否则就变成 hard link了。
>
>这个思想好像就是我在想的为什么要给目录底下的每个文件做 link，link到目录的 inode 不就好了嘛
>%%TAGS%%
>#文件系统
^19mhzh3gyjb


>%%
>```annotation-json
>{"created":"2023-12-11T12:01:18.056Z","updated":"2023-12-11T12:01:18.056Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":343421,"end":343430},{"type":"TextQuoteSelector","exact":"建立一个独立的文件","prefix":" 可就好理解多了，基本上， Symbolic link  就是在","suffix":"，而这个文件会让数据的读取指向他  link  的那个文件的档名"}]}]}
>```
>%%
>*%%PREFIX%%可就好理解多了，基本上， Symbolic link  就是在%%HIGHLIGHT%% ==建立一个独立的文件== %%POSTFIX%%，而这个文件会让数据的读取指向他  link  的那个文件的档名*
>%%LINK%%[[#^y0pw6x4kvt9|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^y0pw6x4kvt9


>%%
>```annotation-json
>{"created":"2023-12-11T12:06:26.702Z","updated":"2023-12-11T12:06:26.702Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":346761,"end":346776},{"type":"TextQuoteSelector","exact":"/tmp  这个目录是干嘛用的","prefix":"有特殊的颜色显示喔！ Tips 还记得第五章当中，我们提到的  ","suffix":"吗？是给大家作为暂存盘用的啊！  所以，您会发现，过去我们在进行"}]}]}
>```
>%%
>*%%PREFIX%%有特殊的颜色显示喔！ Tips 还记得第五章当中，我们提到的%%HIGHLIGHT%% ==/tmp  这个目录是干嘛用的== %%POSTFIX%%吗？是给大家作为暂存盘用的啊！  所以，您会发现，过去我们在进行*
>%%LINK%%[[#^mskx86t89im|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^mskx86t89im


>%%
>```annotation-json
>{"created":"2023-12-11T12:07:03.311Z","text":"所以说在路径中 / 跟 /root 其实是一个东西是吧","updated":"2023-12-11T12:07:03.311Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":347395,"end":347413},{"type":"TextQuoteSelector","exact":"该目录其实是  /bin  这个目录","prefix":"那么如果你进入  /root/bin  这个目录下，『请注意呦！","suffix":"，因为你做了连结档了！』所以，如果你进入  /root/bin "}]}]}
>```
>%%
>*%%PREFIX%%那么如果你进入  /root/bin  这个目录下，『请注意呦！%%HIGHLIGHT%% ==该目录其实是  /bin  这个目录== %%POSTFIX%%，因为你做了连结档了！』所以，如果你进入  /root/bin*
>%%LINK%%[[#^6ag2ibdwfnm|show annotation]]
>%%COMMENT%%
>所以说在路径中 / 跟 /root 其实是一个东西是吧
>%%TAGS%%
>#文件系统
^6ag2ibdwfnm


>%%
>```annotation-json
>{"created":"2023-12-13T08:27:32.024Z","updated":"2023-12-13T08:27:32.024Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":412343,"end":412379},{"type":"TextQuoteSelector","exact":"压缩技术会记录为『100 个 1』而不是真的有 100 个 1 的位存在","prefix":"果你的数据为『111....』共有 100 个 1 时，  那么","suffix":"！这样也能够精简文件记录的容量呢！  非常有趣吧！ 简单的说，你"}]}]}
>```
>%%
>*%%PREFIX%%果你的数据为『111....』共有 100 个 1 时，  那么%%HIGHLIGHT%% ==压缩技术会记录为『100 个 1』而不是真的有 100 个 1 的位存在== %%POSTFIX%%！这样也能够精简文件记录的容量呢！  非常有趣吧！ 简单的说，你*
>%%LINK%%[[#^59jjnwxdocu|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#压缩
^59jjnwxdocu


>%%
>```annotation-json
>{"created":"2023-12-13T08:27:38.785Z","updated":"2023-12-13T08:27:38.785Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":412236,"end":412264},{"type":"TextQuoteSelector","exact":"将这些没有使用到的空间『丢』出来，以让文件占用的空间变小","prefix":"来记录了！而一些聪明的计算机工程师就利用一些复杂的计算方式，  ","suffix":"！这就是压缩的技术啦！ 另外一种压缩技术也很有趣，他是将重复的数"}]}]}
>```
>%%
>*%%PREFIX%%来记录了！而一些聪明的计算机工程师就利用一些复杂的计算方式，%%HIGHLIGHT%% ==将这些没有使用到的空间『丢』出来，以让文件占用的空间变小== %%POSTFIX%%！这就是压缩的技术啦！ 另外一种压缩技术也很有趣，他是将重复的数*
>%%LINK%%[[#^mxvync4xdyo|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#压缩
^mxvync4xdyo


>%%
>```annotation-json
>{"created":"2023-12-13T08:32:08.194Z","updated":"2023-12-13T08:32:08.194Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":413507,"end":413619},{"type":"TextQuoteSelector","exact":"Linux  支持的压缩指令非常多，且不同的指令所用的压缩技术并不相同，当然彼此之间可能就无法互通压缩/解压缩文件案啰。  所以，当你下载到某个压缩文件时，自然就需要知道该文件是由哪种压缩指令所制作出来的，好用来对照着解压缩","prefix":"？不是说  Linux  的扩展名没有什么作用吗？ 这是因为  ","suffix":"啊！  也就是说，虽然  Linux  文件的属性基本上是与文件"}]}]}
>```
>%%
>*%%PREFIX%%？不是说  Linux  的扩展名没有什么作用吗？ 这是因为%%HIGHLIGHT%% ==Linux  支持的压缩指令非常多，且不同的指令所用的压缩技术并不相同，当然彼此之间可能就无法互通压缩/解压缩文件案啰。  所以，当你下载到某个压缩文件时，自然就需要知道该文件是由哪种压缩指令所制作出来的，好用来对照着解压缩== %%POSTFIX%%啊！  也就是说，虽然  Linux  文件的属性基本上是与文件*
>%%LINK%%[[#^edkv2rgydbp|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#压缩
^edkv2rgydbp


>%%
>```annotation-json
>{"created":"2023-12-13T08:33:40.359Z","text":"他不是一种压缩方式，而是一种打包方式","updated":"2023-12-13T08:33:40.359Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":414294,"end":414317},{"type":"TextQuoteSelector","exact":" tar  可以将很多文件『打包』成为一个文件","prefix":"？此时，那个所谓的『打包软件, tar』就显的很重要啦！ 这个 ","suffix":"！甚至是目录也可以这么玩。不过，单纯的  tar  功能仅是『打"}]}]}
>```
>%%
>*%%PREFIX%%？此时，那个所谓的『打包软件, tar』就显的很重要啦！ 这个%%HIGHLIGHT%% ==tar  可以将很多文件『打包』成为一个文件== %%POSTFIX%%！甚至是目录也可以这么玩。不过，单纯的  tar  功能仅是『打*
>%%LINK%%[[#^mer991qw6bf|show annotation]]
>%%COMMENT%%
>他不是一种压缩方式，而是一种打包方式
>%%TAGS%%
>#压缩
^mer991qw6bf


>%%
>```annotation-json
>{"created":"2023-12-13T08:36:47.621Z","updated":"2023-12-13T08:36:47.621Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":415575,"end":415584},{"type":"TextQuoteSelector","exact":"源文件就不再存在了","prefix":"缩时，在预设的状态下原本的文件会被压缩成为  .gz  的档名，","suffix":"。  这点与一般习惯使用  windows  做压缩的朋友所熟悉"}]}]}
>```
>%%
>*%%PREFIX%%缩时，在预设的状态下原本的文件会被压缩成为  .gz  的档名，%%HIGHLIGHT%% ==源文件就不再存在了== %%POSTFIX%%。  这点与一般习惯使用  windows  做压缩的朋友所熟悉*
>%%LINK%%[[#^95m2in46ar8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^95m2in46ar8


>%%
>```annotation-json
>{"created":"2023-12-13T08:37:57.212Z","text":"不用真正解压文件，就能显示压缩文件中的内容","updated":"2023-12-13T08:37:57.212Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":415772,"end":415776},{"type":"TextQuoteSelector","exact":"zcat","prefix":"压缩文件的内容读出来！ [dmtsai@study tmp]$ ","suffix":" services.gz # 由于 services 这个原本的"}]}]}
>```
>%%
>*%%PREFIX%%压缩文件的内容读出来！ [dmtsai@study tmp]$%%HIGHLIGHT%% ==zcat== %%POSTFIX%%services.gz # 由于 services 这个原本的*
>%%LINK%%[[#^wev7y0d7rd|show annotation]]
>%%COMMENT%%
>不用真正解压文件，就能显示压缩文件中的内容
>%%TAGS%%
>#压缩
^wev7y0d7rd



>%%
>```annotation-json
>{"created":"2023-12-13T08:42:51.525Z","text":"将数据重新定向，从而不丢失源文件，有点像 tube 的作用。\n朴素的做法，将数据拷贝之后再压缩。","updated":"2023-12-13T08:42:51.525Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":416576,"end":416674},{"type":"TextQuoteSelector","exact":"-c  可以将原本要转成压缩文件的资料内容，将它变成文字类型从屏幕输出，  然后我们可以透过大于 (>)  这个符号，将原本应该由屏幕输出的数据，转成输出到文件而不是屏幕，所以就能够建立出压缩挡了","prefix":"  的选项。范例四的重点在那个  -c  与  >  的使用啰！","suffix":"。只是档名也要自己写，  当然最好还是遵循  gzip  的压缩"}]}]}
>```
>%%
>*%%PREFIX%%的选项。范例四的重点在那个  -c  与  >  的使用啰！%%HIGHLIGHT%% ==-c  可以将原本要转成压缩文件的资料内容，将它变成文字类型从屏幕输出，  然后我们可以透过大于 (>)  这个符号，将原本应该由屏幕输出的数据，转成输出到文件而不是屏幕，所以就能够建立出压缩挡了== %%POSTFIX%%。只是档名也要自己写，  当然最好还是遵循  gzip  的压缩*
>%%LINK%%[[#^1iuiu63cufjk|show annotation]]
>%%COMMENT%%
>将数据重新定向，从而不丢失源文件，有点像 tube 的作用。
>朴素的做法，将数据拷贝之后再压缩。
>%%TAGS%%
>#压缩
^1iuiu63cufjk


>%%
>```annotation-json
>{"created":"2023-12-13T08:44:41.783Z","updated":"2023-12-13T08:44:41.783Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":416752,"end":416847},{"type":"TextQuoteSelector","exact":"cat/more/less  可以使用不同的方式来读取纯文本档，那个  zcat/zmore/zless  则可以对应于 cat/more/less  的方式来读取纯文本档被压缩后的压缩文件","prefix":" >  这个符号的应用，我们会在  bash  章节再次提及！ ","suffix":"！  由于  gzip  这个压缩指令主要想要用来取代  com"}]}]}
>```
>%%
>*%%PREFIX%%>  这个符号的应用，我们会在  bash  章节再次提及！%%HIGHLIGHT%% ==cat/more/less  可以使用不同的方式来读取纯文本档，那个  zcat/zmore/zless  则可以对应于 cat/more/less  的方式来读取纯文本档被压缩后的压缩文件== %%POSTFIX%%！  由于  gzip  这个压缩指令主要想要用来取代  com*
>%%LINK%%[[#^g8fqm49qg8j|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^g8fqm49qg8j


>%%
>```annotation-json
>{"created":"2023-12-13T08:44:45.539Z","text":"compress 压缩文件后缀为 .Z","updated":"2023-12-13T08:44:45.539Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":416854,"end":416887},{"type":"TextQuoteSelector","exact":"gzip  这个压缩指令主要想要用来取代  compress  的","prefix":"less  的方式来读取纯文本档被压缩后的压缩文件！  由于  ","suffix":"，所以不但  compress  的压缩文件案可以使用  gzi"}]}]}
>```
>%%
>*%%PREFIX%%less  的方式来读取纯文本档被压缩后的压缩文件！  由于%%HIGHLIGHT%% ==gzip  这个压缩指令主要想要用来取代  compress  的== %%POSTFIX%%，所以不但  compress  的压缩文件案可以使用  gzi*
>%%LINK%%[[#^jaf9m8i1fxe|show annotation]]
>%%COMMENT%%
>compress 压缩文件后缀为 .Z
>%%TAGS%%
>#压缩
^jaf9m8i1fxe


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":417182,"end":417207},{"type":"TextQuoteSelector","exact":"znew  可以将该文件转成  gzip  的格示","prefix":"press  建置出来的  .Z  文件，那也无须担心，使用","suffix":"喔！ 8.2.2 bzip2, bzcat/bzmore/bzl"}]}],"created":"2023-12-13T08:45:54.503Z","updated":"2023-12-13T08:45:54.503Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%press  建置出来的  .Z  文件，那也无须担心，使用%%HIGHLIGHT%% ==znew  可以将该文件转成  gzip  的格示== %%POSTFIX%%喔！ 8.2.2 bzip2, bzcat/bzmore/bzl*
>%%LINK%%[[#^xltecnr3xl9|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#压缩
^xltecnr3xl9


>%%
>```annotation-json
>{"created":"2023-12-13T16:18:22.100Z","updated":"2023-12-13T16:18:22.100Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":417352,"end":417396},{"type":"TextQuoteSelector","exact":"压缩比竟然比  gzip  还要好～至于 bzip2  的用法几乎与  gzip  相同","prefix":"佳的压缩比而来的。  bzip2  真是很不错用的东西～这玩意的","suffix":"！看看底下的用法吧！ [dmtsai@study ~]$ bzi"}]}]}
>```
>%%
>*%%PREFIX%%佳的压缩比而来的。  bzip2  真是很不错用的东西～这玩意的%%HIGHLIGHT%% ==压缩比竟然比  gzip  还要好～至于 bzip2  的用法几乎与  gzip  相同== %%POSTFIX%%！看看底下的用法吧！ [dmtsai@study ~]$ bzi*
>%%LINK%%[[#^d6o66vdmwgi|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#压缩
^d6o66vdmwgi


>%%
>```annotation-json
>{"created":"2023-12-13T16:19:58.072Z","updated":"2023-12-13T16:19:58.072Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":419597,"end":419613},{"type":"TextQuoteSelector","exact":"xz  这个压缩比真的好太多太多","prefix":"@study tmp]$ xz -k services 虽然  ","suffix":"了！以鸟哥选择的这个  services  文件为范例，他可以将"}]}]}
>```
>%%
>*%%PREFIX%%@study tmp]$ xz -k services 虽然%%HIGHLIGHT%% ==xz  这个压缩比真的好太多太多== %%POSTFIX%%了！以鸟哥选择的这个  services  文件为范例，他可以将*
>%%LINK%%[[#^rnow0ojmnra|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#压缩
^rnow0ojmnra


>%%
>```annotation-json
>{"created":"2023-12-13T16:20:38.184Z","updated":"2023-12-13T16:20:38.184Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":419720,"end":419725},{"type":"TextQuoteSelector","exact":"时间花太久","prefix":"%  耶！  差非常非常多！不过，  xz  最大的问题是...","suffix":"了！如果你曾经使用过  xz  的话，应该会有发现，他的运算时间"}]}]}
>```
>%%
>*%%PREFIX%%%  耶！  差非常非常多！不过，  xz  最大的问题是...%%HIGHLIGHT%% ==时间花太久== %%POSTFIX%%了！如果你曾经使用过  xz  的话，应该会有发现，他的运算时间*
>%%LINK%%[[#^28njc290yur|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^28njc290yur


>%%
>```annotation-json
>{"created":"2023-12-13T16:21:39.218Z","updated":"2023-12-13T16:21:39.218Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":420115,"end":420173},{"type":"TextQuoteSelector","exact":"不像在  Windows  的系统，可以使用类似 WinRAR 这一类的压缩软件来将好多数据『包成一个文件』的样式。","prefix":"缩指的是『将目录内的所有文件  \"分别\"  进行压缩』的动作！而","suffix":" 这种将多个文件或目录包成一个大文件的指令功能，我们可以称呼他是"}]}]}
>```
>%%
>*%%PREFIX%%缩指的是『将目录内的所有文件  "分别"  进行压缩』的动作！而%%HIGHLIGHT%% ==不像在  Windows  的系统，可以使用类似 WinRAR 这一类的压缩软件来将好多数据『包成一个文件』的样式。== %%POSTFIX%%这种将多个文件或目录包成一个大文件的指令功能，我们可以称呼他是*
>%%LINK%%[[#^6s2jviulwrd|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#压缩
^6s2jviulwrd


>%%
>```annotation-json
>{"created":"2023-12-13T16:24:07.653Z","text":"tar 的三种不同模式","updated":"2023-12-13T16:24:07.653Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":420838,"end":420863},{"type":"TextQuoteSelector","exact":"-c, -t, -x 不可同时出现在一串指令列中。","prefix":"配 -C (大写) 在特定目录解开       特别留意的是， ","suffix":" -z  ：透过 gzip  的支持进行压缩/解压缩：此时档名最"}]}]}
>```
>%%
>*%%PREFIX%%配 -C (大写) 在特定目录解开       特别留意的是，%%HIGHLIGHT%% ==-c, -t, -x 不可同时出现在一串指令列中。== %%POSTFIX%%-z  ：透过 gzip  的支持进行压缩/解压缩：此时档名最*
>%%LINK%%[[#^bpy6xz8zhw4|show annotation]]
>%%COMMENT%%
>tar 的三种不同模式
>%%TAGS%%
>#压缩
^bpy6xz8zhw4


>%%
>```annotation-json
>{"created":"2023-12-13T16:24:57.553Z","text":"注意，档名是自己设定的，目的是告诉别人应该用什么工具去解压缩，系统本身不会强制你去用什么档名噢","updated":"2023-12-13T16:24:57.553Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":420890,"end":420907},{"type":"TextQuoteSelector","exact":"此时档名最好为 *.tar.gz ","prefix":"指令列中。 -z  ：透过 gzip  的支持进行压缩/解压缩：","suffix":"-j  ：透过 bzip2 的支持进行压缩/解压缩：此时档名最好"}]}]}
>```
>%%
>*%%PREFIX%%指令列中。 -z  ：透过 gzip  的支持进行压缩/解压缩：%%HIGHLIGHT%% ==此时档名最好为 *.tar.gz== %%POSTFIX%%-j  ：透过 bzip2 的支持进行压缩/解压缩：此时档名最好*
>%%LINK%%[[#^q0i7v88regi|show annotation]]
>%%COMMENT%%
>注意，档名是自己设定的，目的是告诉别人应该用什么工具去解压缩，系统本身不会强制你去用什么档名噢
>%%TAGS%%
>#压缩
^q0i7v88regi


>%%
>```annotation-json
>{"created":"2023-12-13T16:28:10.867Z","text":"承上。\n所以只打包不压缩是什么效果呢？","updated":"2023-12-13T16:28:10.867Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":421480,"end":421556},{"type":"TextQuoteSelector","exact":"tar  并不会主动的产生建立的档名喔！我们要自定义啦！ 所以扩展名就显的很重要了！如果不加  [-z|-j|-J]  的话，档名最好取为  *.tar","prefix":"那个  filename.tar.bz2  是我们自己取的档名，","suffix":"  即可。如果是  -j  选项，代表有  bzip2  的支持"}]}]}
>```
>%%
>*%%PREFIX%%那个  filename.tar.bz2  是我们自己取的档名，%%HIGHLIGHT%% ==tar  并不会主动的产生建立的档名喔！我们要自定义啦！ 所以扩展名就显的很重要了！如果不加  [-z|-j|-J]  的话，档名最好取为  *.tar== %%POSTFIX%%即可。如果是  -j  选项，代表有  bzip2  的支持*
>%%LINK%%[[#^ibakqq01gg|show annotation]]
>%%COMMENT%%
>承上。
>所以只打包不压缩是什么效果呢？
>%%TAGS%%
>#压缩
^ibakqq01gg


>%%
>```annotation-json
>{"created":"2023-12-13T16:31:27.634Z","text":"-f 后面要紧接你要生成的文件名","updated":"2023-12-13T16:31:27.634Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":421861,"end":421888},{"type":"TextQuoteSelector","exact":"将『  -f filename  』与其他选项独立出来","prefix":"  因为  -fc  嘛！所以啰，建议您在学习  tar  时，","suffix":"，会比较不容易发生问题。 闲话少说，让我们来测试几个常用的  t"}]}]}
>```
>%%
>*%%PREFIX%%因为  -fc  嘛！所以啰，建议您在学习  tar  时，%%HIGHLIGHT%% ==将『  -f filename  』与其他选项独立出来== %%POSTFIX%%，会比较不容易发生问题。 闲话少说，让我们来测试几个常用的  t*
>%%LINK%%[[#^d49tcqcmnz5|show annotation]]
>%%COMMENT%%
>-f 后面要紧接你要生成的文件名
>%%TAGS%%
>#压缩
^d49tcqcmnz5


>%%
>```annotation-json
>{"created":"2023-12-13T16:36:08.639Z","text":"看上去 tar 的压缩会自己保留原文件","updated":"2023-12-13T16:36:08.639Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":420715,"end":420752},{"type":"TextQuoteSelector","exact":"建立打包文件，可搭配 -v 来察看过程中被打包的档名(filename) ","prefix":"名] [-C 目录]   <==解压缩 选项与参数： -c  ：","suffix":"-t  ：察看打包文件的内容含有哪些档名，重点在察看『档名』就是"}]}]}
>```
>%%
>*%%PREFIX%%名] [-C 目录]   <==解压缩 选项与参数： -c  ：%%HIGHLIGHT%% ==建立打包文件，可搭配 -v 来察看过程中被打包的档名(filename)== %%POSTFIX%%-t  ：察看打包文件的内容含有哪些档名，重点在察看『档名』就是*
>%%LINK%%[[#^orsz9ze0epf|show annotation]]
>%%COMMENT%%
>看上去 tar 的压缩会自己保留原文件
>%%TAGS%%
>#压缩
^orsz9ze0epf


>%%
>```annotation-json
>{"created":"2023-12-13T16:38:26.372Z","text":"使你的目录变为相对目录，这样你就可以选择解压后的目录。","updated":"2023-12-13T16:38:26.372Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":423881,"end":424149},{"type":"TextQuoteSelector","exact":"那为什么要拿掉根目录呢？主要是为了安全！我们使用  tar  备份的数据可能会需要解压缩回来使用， 在  tar  所记录的文件名  (就是我们刚刚使用  tar -jtvf  所察看到的檔名)  那就是解压缩后的实际档名。 如果拿掉了根目录，假设你将备份数据在  /tmp  解开，那么解压缩的档名就会变成『/tmp/etc/xxx』。 但『如果没有拿掉根目录，解压缩后的档名就会是绝对路径，  亦即解压缩后的数据一定会被放置到 /etc/xxx 去！』如此一来，你的原本的  /etc/  底下的数据，  就会被备份数据所覆盖过去了","prefix":"r names(移除了档名开头的  `/' )』所告知的情况！ ","suffix":"！ Tips 你会说：『既然是备份数据，那么还原回来也没有什么问"}]}]}
>```
>%%
>*%%PREFIX%%r names(移除了档名开头的  `/' )』所告知的情况！%%HIGHLIGHT%% ==那为什么要拿掉根目录呢？主要是为了安全！我们使用  tar  备份的数据可能会需要解压缩回来使用， 在  tar  所记录的文件名  (就是我们刚刚使用  tar -jtvf  所察看到的檔名)  那就是解压缩后的实际档名。 如果拿掉了根目录，假设你将备份数据在  /tmp  解开，那么解压缩的档名就会变成『/tmp/etc/xxx』。 但『如果没有拿掉根目录，解压缩后的档名就会是绝对路径，  亦即解压缩后的数据一定会被放置到 /etc/xxx 去！』如此一来，你的原本的  /etc/  底下的数据，  就会被备份数据所覆盖过去了== %%POSTFIX%%！ Tips 你会说：『既然是备份数据，那么还原回来也没有什么问*
>%%LINK%%[[#^deorh26fpf6|show annotation]]
>%%COMMENT%%
>使你的目录变为相对目录，这样你就可以选择解压后的目录。
>%%TAGS%%
>#压缩
^deorh26fpf6


>%%
>```annotation-json
>{"created":"2023-12-13T16:40:25.148Z","text":"比较危险","updated":"2023-12-13T16:40:25.148Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":421216,"end":421250},{"type":"TextQuoteSelector","exact":"-P(大写) ：保留绝对路径，亦即允许备份数据中含有根目录存在之意；","prefix":"保留备份数据的原本权限与属性，常用于备份(-c)重要的配置文件 ","suffix":" --exclude=FILE：在压缩的过程中，不要将 FILE"}]}]}
>```
>%%
>*%%PREFIX%%保留备份数据的原本权限与属性，常用于备份(-c)重要的配置文件%%HIGHLIGHT%% ==-P(大写) ：保留绝对路径，亦即允许备份数据中含有根目录存在之意；== %%POSTFIX%%--exclude=FILE：在压缩的过程中，不要将 FILE*
>%%LINK%%[[#^wh89nbxl7b|show annotation]]
>%%COMMENT%%
>比较危险
>%%TAGS%%
>#压缩
^wh89nbxl7b



>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":428561,"end":428616},{"type":"TextQuoteSelector","exact":"仅是打包而已，就是『  tar -cv -f file.tar  』而已，这个文件我们称呼为  tarfile","prefix":"r  打包出来的文件有没有进行压缩所得到文件称呼不同喔！  如果","suffix":"。 如果还有进行压缩的支持，例如『  tar -jcv -f"}]}],"created":"2023-12-13T16:46:39.220Z","updated":"2023-12-13T16:46:39.220Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%r  打包出来的文件有没有进行压缩所得到文件称呼不同喔！  如果%%HIGHLIGHT%% ==仅是打包而已，就是『  tar -cv -f file.tar  』而已，这个文件我们称呼为  tarfile== %%POSTFIX%%。 如果还有进行压缩的支持，例如『  tar -jcv -f*
>%%LINK%%[[#^iwfetxqg98|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^iwfetxqg98


>%%
>```annotation-json
>{"target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":428619,"end":428682},{"type":"TextQuoteSelector","exact":" 如果还有进行压缩的支持，例如『  tar -jcv -f file.tar.bz2  』时，我们就称呼为  tarball ","prefix":"e.tar  』而已，这个文件我们称呼为  tarfile  。","suffix":"(tar  球？)！这只是一个基本的称谓而已，不过很多书籍与网络"}]}],"created":"2023-12-13T16:46:47.559Z","updated":"2023-12-13T16:46:47.559Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf"}
>```
>%%
>*%%PREFIX%%e.tar  』而已，这个文件我们称呼为  tarfile  。%%HIGHLIGHT%% ==如果还有进行压缩的支持，例如『  tar -jcv -f file.tar.bz2  』时，我们就称呼为  tarball== %%POSTFIX%%(tar  球？)！这只是一个基本的称谓而已，不过很多书籍与网络*
>%%LINK%%[[#^lrm8csg0cg|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^lrm8csg0cg


>%%
>```annotation-json
>{"created":"2023-12-14T04:52:47.449Z","updated":"2023-12-14T04:52:47.449Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":466204,"end":466220},{"type":"TextQuoteSelector","exact":"修改与设定某些重要软件的配置文件","prefix":"最近更新日期：2015/07/07 系统管理员的重要工作就是得要","suffix":"，因此至少得要学会一种以上的文字接口的文书编辑器。  在所有的 "}]}]}
>```
>%%
>*%%PREFIX%%最近更新日期：2015/07/07 系统管理员的重要工作就是得要%%HIGHLIGHT%% ==修改与设定某些重要软件的配置文件== %%POSTFIX%%，因此至少得要学会一种以上的文字接口的文书编辑器。  在所有的*
>%%LINK%%[[#^fmnut3icyr|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^fmnut3icyr


>%%
>```annotation-json
>{"created":"2023-12-14T04:56:32.401Z","updated":"2023-12-14T04:56:32.401Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":466922,"end":466966},{"type":"TextQuoteSelector","exact":"在  Linux  的世界中，绝大部分的配置文件都是以  ASCII  的纯文本形态存在","prefix":"nux distributions  时，呵呵！那可就苦恼了！ ","suffix":"，因此利用简单的文字编辑软件就能够修改设定了！  与微软的  W"}]}]}
>```
>%%
>*%%PREFIX%%nux distributions  时，呵呵！那可就苦恼了！%%HIGHLIGHT%% ==在  Linux  的世界中，绝大部分的配置文件都是以  ASCII  的纯文本形态存在== %%POSTFIX%%，因此利用简单的文字编辑软件就能够修改设定了！  与微软的  W*
>%%LINK%%[[#^mamiso53br8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^mamiso53br8


>%%
>```annotation-json
>{"created":"2023-12-14T08:13:37.617Z","updated":"2023-12-14T08:13:37.617Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":468114,"end":468119},{"type":"TextQuoteSelector","exact":"程序编辑器","prefix":"来显示程序代码与一般信息。也就是说，  这个  vim  是个『","suffix":"』啦！甚至一些  Linux  基础配置文件内的语法，都能够用 "}]}]}
>```
>%%
>*%%PREFIX%%来显示程序代码与一般信息。也就是说，  这个  vim  是个『%%HIGHLIGHT%% ==程序编辑器== %%POSTFIX%%』啦！甚至一些  Linux  基础配置文件内的语法，都能够用*
>%%LINK%%[[#^7kmq2dwm8vh|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^7kmq2dwm8vh


>%%
>```annotation-json
>{"created":"2023-12-14T08:24:46.767Z","updated":"2023-12-14T08:24:46.767Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":467648,"end":467669},{"type":"TextQuoteSelector","exact":"很多个别软件的编辑接口都会主动呼叫  vi","prefix":"建  vi  文书编辑器，其他的文书编辑器则不一定会存在；  ","suffix":" (例如未来会谈到的 crontab, visudo, edqu"}]}]}
>```
>%%
>*%%PREFIX%%建  vi  文书编辑器，其他的文书编辑器则不一定会存在； %%HIGHLIGHT%% ==很多个别软件的编辑接口都会主动呼叫  vi== %%POSTFIX%%(例如未来会谈到的 crontab, visudo, edqu*
>%%LINK%%[[#^nn6ut89mod|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^nn6ut89mod


>%%
>```annotation-json
>{"created":"2023-12-14T08:27:45.966Z","updated":"2023-12-14T08:27:45.966Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":469352,"end":469394},{"type":"TextQuoteSelector","exact":"一般指令模式可与编辑模式及指令列模式切换，  但编辑模式与指令列模式之间不可互相切换","prefix":"9.2.1、vi 三种模式的相互关系 注意到上面的图标，你会发现","suffix":"喔！这非常重要啦！闲话不多说，我们底下以一个简单的例子来进行说明"}]}]}
>```
>%%
>*%%PREFIX%%9.2.1、vi 三种模式的相互关系 注意到上面的图标，你会发现%%HIGHLIGHT%% ==一般指令模式可与编辑模式及指令列模式切换，  但编辑模式与指令列模式之间不可互相切换== %%POSTFIX%%喔！这非常重要啦！闲话不多说，我们底下以一个简单的例子来进行说明*
>%%LINK%%[[#^janht5ezms|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^janht5ezms


>%%
>```annotation-json
>{"created":"2023-12-14T08:32:41.544Z","text":"有改变文件权限的权限","updated":"2023-12-14T08:32:41.544Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":471082,"end":471137},{"type":"TextQuoteSelector","exact":"使用『 :wq! 』 多加一个惊叹号即可！不过，需要特别注意呦！那个是在『你的权限可以改变』的情况下才能成立的","prefix":"时，那么可能会无法写入，此时可以使用『强制写入』的方式吗？可以！","suffix":"！ 关于权限的概念，请自行回去翻一下第五章的内容吧！ 9.2.2"}]}]}
>```
>%%
>*%%PREFIX%%时，那么可能会无法写入，此时可以使用『强制写入』的方式吗？可以！%%HIGHLIGHT%% ==使用『 :wq! 』 多加一个惊叹号即可！不过，需要特别注意呦！那个是在『你的权限可以改变』的情况下才能成立的== %%POSTFIX%%！ 关于权限的概念，请自行回去翻一下第五章的内容吧！ 9.2.2*
>%%LINK%%[[#^dsjudpe2ly9|show annotation]]
>%%COMMENT%%
>有改变文件权限的权限
>%%TAGS%%
>#vim
^dsjudpe2ly9


>%%
>```annotation-json
>{"created":"2023-12-14T16:26:30.237Z","updated":"2023-12-14T16:26:30.237Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":474390,"end":474417},{"type":"TextQuoteSelector","exact":"惊叹号 (!) 在 vi 当中，常常具有『强制』的意思","prefix":"，又不想储存，使用 ! 为强制离开不储存文件。 注意一下啊，那个","suffix":"～ :wq 储存后离开，若为 :wq! 则为强制储存后离开 (常"}]}]}
>```
>%%
>*%%PREFIX%%，又不想储存，使用 ! 为强制离开不储存文件。 注意一下啊，那个%%HIGHLIGHT%% ==惊叹号 (!) 在 vi 当中，常常具有『强制』的意思== %%POSTFIX%%～ :wq 储存后离开，若为 :wq! 则为强制储存后离开 (常*
>%%LINK%%[[#^ix73tui0ng|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^ix73tui0ng


>%%
>```annotation-json
>{"created":"2023-12-14T16:29:08.040Z","text":"在 vim 中你可以将很多命令创意的组合起来，以获得超越单条命令的效果。","updated":"2023-12-14T16:29:08.040Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":474831,"end":474856},{"type":"TextQuoteSelector","exact":"『数字』是很有意义的！数字通常代表重复做几次的意思","prefix":" set nu 相反，为取消行号！ 特别注意，在  vi  中，","suffix":"！  也有可能是代表去到第几个什么什么的意思。举例来说，要删除 "}]}]}
>```
>%%
>*%%PREFIX%%set nu 相反，为取消行号！ 特别注意，在  vi  中，%%HIGHLIGHT%% ==『数字』是很有意义的！数字通常代表重复做几次的意思== %%POSTFIX%%！  也有可能是代表去到第几个什么什么的意思。举例来说，要删除*
>%%LINK%%[[#^lrrvqwfw7|show annotation]]
>%%COMMENT%%
>在 vim 中你可以将很多命令创意的组合起来，以获得超越单条命令的效果。
>%%TAGS%%
>#vim
^lrrvqwfw7


>%%
>```annotation-json
>{"created":"2023-12-14T16:35:30.867Z","updated":"2023-12-14T16:35:30.867Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":476780,"end":476847},{"type":"TextQuoteSelector","exact":"都会有『回复』的功能，亦即当你的系统因为某些原因而导致类似当机的情况时，  还可以透过某些特别的机制来让你将之前未储存的数据『救』回来","prefix":" 的暂存档、救援回复与开启时的警告讯息 在目前主要的文书编辑软件","suffix":"！这就是鸟哥这里所谓的『回复』功能啦！  那么  vim  有没"}]}]}
>```
>%%
>*%%PREFIX%%的暂存档、救援回复与开启时的警告讯息 在目前主要的文书编辑软件%%HIGHLIGHT%% ==都会有『回复』的功能，亦即当你的系统因为某些原因而导致类似当机的情况时，  还可以透过某些特别的机制来让你将之前未储存的数据『救』回来== %%POSTFIX%%！这就是鸟哥这里所谓的『回复』功能啦！  那么  vim  有没*
>%%LINK%%[[#^3fnr3rx27ho|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^3fnr3rx27ho


>%%
>```annotation-json
>{"created":"2023-12-14T16:38:40.065Z","text":"正常退出的情况下这个文件会自动删除。\n","updated":"2023-12-14T16:38:40.065Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":476916,"end":476977},{"type":"TextQuoteSelector","exact":"使用  vim  编辑时，  vim  会在与被编辑的文件的目录下，再建立一个名为  .filename.swp  的文件","prefix":"呢？有的！  vim  就是透过『暂存档』来救援的啦！ 当我们在","suffix":"。  比如说我们在上一个小节谈到的编辑  /tmp/vitest"}]}]}
>```
>%%
>*%%PREFIX%%呢？有的！  vim  就是透过『暂存档』来救援的啦！ 当我们在%%HIGHLIGHT%% ==使用  vim  编辑时，  vim  会在与被编辑的文件的目录下，再建立一个名为  .filename.swp  的文件== %%POSTFIX%%。  比如说我们在上一个小节谈到的编辑  /tmp/vitest*
>%%LINK%%[[#^mkjq3uy3x97|show annotation]]
>%%COMMENT%%
>正常退出的情况下这个文件会自动删除。
>
>%%TAGS%%
>#vim
^mkjq3uy3x97


>%%
>```annotation-json
>{"created":"2023-12-14T16:41:08.693Z","updated":"2023-12-14T16:41:08.693Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":480825,"end":480862},{"type":"TextQuoteSelector","exact":"vim  具有颜色显示的功能，并且还支持许多的程序语法  (syntax)","prefix":"经被  vim  所取代啰～为什么要用  vim  呢？因为  ","suffix":"，  因此，当你使用  vim  编辑程序时  (不论是  C "}]}]}
>```
>%%
>*%%PREFIX%%经被  vim  所取代啰～为什么要用  vim  呢？因为%%HIGHLIGHT%% ==vim  具有颜色显示的功能，并且还支持许多的程序语法  (syntax)== %%POSTFIX%%，  因此，当你使用  vim  编辑程序时  (不论是  C*
>%%LINK%%[[#^e6nizo4brtr|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^e6nizo4brtr


>%%
>```annotation-json
>{"created":"2023-12-14T16:42:31.735Z","text":"化名\n","updated":"2023-12-14T16:42:31.735Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":480979,"end":480984},{"type":"TextQuoteSelector","exact":"alias","prefix":"g)』的功能！真的很不赖吧！^_^ 如果你在文本模式下，输入  ","suffix":"  时，出现这样的画面： [dmtsai@study ~]$ a"}]}]}
>```
>%%
>*%%PREFIX%%g)』的功能！真的很不赖吧！^_^ 如果你在文本模式下，输入%%HIGHLIGHT%% ==alias== %%POSTFIX%%时，出现这样的画面： [dmtsai@study ~]$ a*
>%%LINK%%[[#^3xbb0wikpwj|show annotation]]
>%%COMMENT%%
>化名
>
>%%TAGS%%
>
^3xbb0wikpwj


>%%
>```annotation-json
>{"created":"2023-12-14T16:54:05.280Z","text":"大写大多有往上、往前的含义","updated":"2023-12-14T16:54:05.280Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":472418,"end":472419},{"type":"TextQuoteSelector","exact":"N","prefix":"，那么按下 n 则会向上继续搜寻名称为 vbird 的字符串！ ","suffix":" 这个 N 是英文按键。与 n 刚好相反，为『反向』进行前一个搜"}]}]}
>```
>%%
>*%%PREFIX%%，那么按下 n 则会向上继续搜寻名称为 vbird 的字符串！%%HIGHLIGHT%% ==N== %%POSTFIX%%这个 N 是英文按键。与 n 刚好相反，为『反向』进行前一个搜*
>%%LINK%%[[#^8gy4rqlvxne|show annotation]]
>%%COMMENT%%
>大写大多有往上、往前的含义
>%%TAGS%%
>#vim
^8gy4rqlvxne


>%%
>```annotation-json
>{"created":"2023-12-14T16:56:23.189Z","text":"separate","updated":"2023-12-14T16:56:23.189Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":484221,"end":484223},{"type":"TextQuoteSelector","exact":"sp","prefix":"但是如何分区窗口并放入文件呢？  很简单啊！在指令列模式输入『:","suffix":" {filename}』即可！那个  filename  可有可"}]}]}
>```
>%%
>*%%PREFIX%%但是如何分区窗口并放入文件呢？  很简单啊！在指令列模式输入『:%%HIGHLIGHT%% ==sp== %%POSTFIX%%{filename}』即可！那个  filename  可有可*
>%%LINK%%[[#^xjidlfj5c97|show annotation]]
>%%COMMENT%%
>separate
>%%TAGS%%
>#vim
^xjidlfj5c97


>%%
>```annotation-json
>{"created":"2023-12-14T16:58:31.221Z","text":"vim 自动判断你的编程语言，予以补齐\n文件拓展名一定要正确","updated":"2023-12-14T16:58:31.221Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":485610,"end":485621},{"type":"TextQuoteSelector","exact":"vim  内建的关键词","prefix":"rl]+x -> [ctrl]+o 以扩展名作为语法补充，以  ","suffix":"，予以补齐 在鸟哥的认知中，比较有用的是第 1, 3  这两个组"}]}]}
>```
>%%
>*%%PREFIX%%rl]+x -> [ctrl]+o 以扩展名作为语法补充，以%%HIGHLIGHT%% ==vim  内建的关键词== %%POSTFIX%%，予以补齐 在鸟哥的认知中，比较有用的是第 1, 3  这两个组*
>%%LINK%%[[#^5250gp02mli|show annotation]]
>%%COMMENT%%
>vim 自动判断你的编程语言，予以补齐
>文件拓展名一定要正确
>%%TAGS%%
>#vim
^5250gp02mli


>%%
>```annotation-json
>{"created":"2023-12-14T16:59:09.708Z","text":"你自己定义的，像是变量名那些？","updated":"2023-12-14T16:59:09.708Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":485512,"end":485519},{"type":"TextQuoteSelector","exact":"文件的内容文字","prefix":"ctrl]+x -> [ctrl]+n 透过目前正在编辑的这个『","suffix":"』作为关键词，予以补齐 [ctrl]+x -> [ctrl]+f"}]}]}
>```
>%%
>*%%PREFIX%%ctrl]+x -> [ctrl]+n 透过目前正在编辑的这个『%%HIGHLIGHT%% ==文件的内容文字== %%POSTFIX%%』作为关键词，予以补齐 [ctrl]+x -> [ctrl]+f*
>%%LINK%%[[#^4we6ty2nj6o|show annotation]]
>%%COMMENT%%
>你自己定义的，像是变量名那些？
>%%TAGS%%
>#vim
^4we6ty2nj6o


>%%
>```annotation-json
>{"created":"2023-12-14T17:02:40.980Z","updated":"2023-12-14T17:02:40.980Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":488137,"end":488188},{"type":"TextQuoteSelector","exact":"/etc/vimrc  这个文件，不过，不建议你修改他！  你可以修改  ~/.vimrc  这个文件","prefix":"vim  操作环境呢！ 整体 vim  的设定值一般是放置在  ","suffix":" (预设不存在，请你自行手动建立！)，将你所希望的设定值写入！ "}]}]}
>```
>%%
>*%%PREFIX%%vim  操作环境呢！ 整体 vim  的设定值一般是放置在%%HIGHLIGHT%% ==/etc/vimrc  这个文件，不过，不建议你修改他！  你可以修改  ~/.vimrc  这个文件== %%POSTFIX%%(预设不存在，请你自行手动建立！)，将你所希望的设定值写入！*
>%%LINK%%[[#^n3tn5mopwr7|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#vim
^n3tn5mopwr7


>%%
>```annotation-json
>{"created":"2023-12-18T06:09:29.630Z","text":"所以我们不直接跟 kernel进行互动，因为我们太危险了","updated":"2023-12-18T06:09:29.630Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":497179,"end":497188},{"type":"TextQuoteSelector","exact":"核心是需要被保护的","prefix":"理整个计算机硬件的其实是操作系统的核心  (kernel)，这个","suffix":"！  所以我们一般使用者就只能透过  shell  来跟核心沟通"}]}]}
>```
>%%
>*%%PREFIX%%理整个计算机硬件的其实是操作系统的核心  (kernel)，这个%%HIGHLIGHT%% ==核心是需要被保护的== %%POSTFIX%%！  所以我们一般使用者就只能透过  shell  来跟核心沟通*
>%%LINK%%[[#^8zrfihwftpb|show annotation]]
>%%COMMENT%%
>所以我们不直接跟 kernel进行互动，因为我们太危险了
>%%TAGS%%
>#shell
^8zrfihwftpb


>%%
>```annotation-json
>{"created":"2023-12-18T06:16:07.203Z","text":"Kernel\n","updated":"2023-12-18T06:16:07.203Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":497872,"end":497945},{"type":"TextQuoteSelector","exact":"操作系统其实是一组软件，由于这组软件在控制整个硬件与管理系统的活动监测，  如果这组软件能被用户随意的操作，若使用者应用不当，将会使得整个系统崩溃","prefix":"心与用户的相关性图示 我们在第零章内的操作系统小节曾经提到过， ","suffix":"！因为操作系统管理的就是整个硬件功能嘛！  所以当然不能够随便被"}]}]}
>```
>%%
>*%%PREFIX%%心与用户的相关性图示 我们在第零章内的操作系统小节曾经提到过，%%HIGHLIGHT%% ==操作系统其实是一组软件，由于这组软件在控制整个硬件与管理系统的活动监测，  如果这组软件能被用户随意的操作，若使用者应用不当，将会使得整个系统崩溃== %%POSTFIX%%！因为操作系统管理的就是整个硬件功能嘛！  所以当然不能够随便被*
>%%LINK%%[[#^zsbgqdwk0d|show annotation]]
>%%COMMENT%%
>Kernel
>
>%%TAGS%%
>#shell
^zsbgqdwk0d


>%%
>```annotation-json
>{"created":"2023-12-18T06:16:44.507Z","text":"包裹在 kernel 外面，保护它免受 shell 的侵害。","updated":"2023-12-18T06:16:44.507Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":498140,"end":498152},{"type":"TextQuoteSelector","exact":"壳程序  (shell)","prefix":"序其实是在最外层，就如同鸡蛋的外壳一样，因此这个咚咚也就被称呼为","suffix":"  啰！ 其实壳程序的功能只是提供用户操作系统的一个接口，因此这"}]}]}
>```
>%%
>*%%PREFIX%%序其实是在最外层，就如同鸡蛋的外壳一样，因此这个咚咚也就被称呼为%%HIGHLIGHT%% ==壳程序  (shell)== %%POSTFIX%%啰！ 其实壳程序的功能只是提供用户操作系统的一个接口，因此这*
>%%LINK%%[[#^hm3nzuk0voc|show annotation]]
>%%COMMENT%%
>包裹在 kernel 外面，保护它免受 shell 的侵害。
>%%TAGS%%
>#shell
^hm3nzuk0voc


>%%
>```annotation-json
>{"created":"2023-12-18T06:18:03.118Z","text":"shell 按照你的指令帮你运行适当的软件，来对 kernel 下达命令","updated":"2023-12-18T06:18:03.118Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":498165,"end":498200},{"type":"TextQuoteSelector","exact":"只是提供用户操作系统的一个接口，因此这个壳程序需要可以呼叫其他软件才好","prefix":"咚也就被称呼为壳程序  (shell)  啰！ 其实壳程序的功能","suffix":"。 我们在第四章到第九章提到过很多指令，包括  man, chm"}]}]}
>```
>%%
>*%%PREFIX%%咚也就被称呼为壳程序  (shell)  啰！ 其实壳程序的功能%%HIGHLIGHT%% ==只是提供用户操作系统的一个接口，因此这个壳程序需要可以呼叫其他软件才好== %%POSTFIX%%。 我们在第四章到第九章提到过很多指令，包括  man, chm*
>%%LINK%%[[#^rzotjf6snnj|show annotation]]
>%%COMMENT%%
>shell 按照你的指令帮你运行适当的软件，来对 kernel 下达命令
>%%TAGS%%
>#shell
^rzotjf6snnj


>%%
>```annotation-json
>{"created":"2023-12-18T06:18:52.917Z","updated":"2023-12-18T06:18:52.917Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":498369,"end":498388},{"type":"TextQuoteSelector","exact":"能够操作应用程序的接口都能够称为壳程序","prefix":" 这样对于壳程序是否有了一定的概念了？ Tips 也就是说，只要","suffix":"。狭义的壳程序指的是指令列方面的软件，包括本章要介绍的  bas"}]}]}
>```
>%%
>*%%PREFIX%%这样对于壳程序是否有了一定的概念了？ Tips 也就是说，只要%%HIGHLIGHT%% ==能够操作应用程序的接口都能够称为壳程序== %%POSTFIX%%。狭义的壳程序指的是指令列方面的软件，包括本章要介绍的  bas*
>%%LINK%%[[#^vlz1t6s9c8f|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#shell
^vlz1t6s9c8f


>%%
>```annotation-json
>{"created":"2023-12-18T06:19:50.707Z","updated":"2023-12-18T06:19:50.707Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":499118,"end":499216},{"type":"TextQuoteSelector","exact":"几乎各家  distributions  使用的  bash  都是一样的！如此一来，  你就能够轻轻松松的转换不同的  distributions  ，就像武侠小说里面提到的『一法通、万法通！』","prefix":"样也造成学习方面的困扰。 文字接口的  shell  就不同了！","suffix":"  远程管理：文字接口就是比较快！ 此外，Linux  的管理"}]}]}
>```
>%%
>*%%PREFIX%%样也造成学习方面的困扰。 文字接口的  shell  就不同了！%%HIGHLIGHT%% ==几乎各家  distributions  使用的  bash  都是一样的！如此一来，  你就能够轻轻松松的转换不同的  distributions  ，就像武侠小说里面提到的『一法通、万法通！』== %%POSTFIX%% 远程管理：文字接口就是比较快！ 此外，Linux  的管理*
>%%LINK%%[[#^6pbjkuzqtfv|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#shell
^6pbjkuzqtfv


>%%
>```annotation-json
>{"created":"2023-12-18T06:20:19.512Z","updated":"2023-12-18T06:20:19.512Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":499263,"end":499301},{"type":"TextQuoteSelector","exact":"文字接口的传输速度一定比较快，  而且，较不容易出现断线或者是信息外流的问题","prefix":"较快！ 此外，Linux  的管理常常需要透过远程联机，而联机时","suffix":"，因此，shell  真的是得学习的一项工具。而且，他可以让您更"}]}]}
>```
>%%
>*%%PREFIX%%较快！ 此外，Linux  的管理常常需要透过远程联机，而联机时%%HIGHLIGHT%% ==文字接口的传输速度一定比较快，  而且，较不容易出现断线或者是信息外流的问题== %%POSTFIX%%，因此，shell  真的是得学习的一项工具。而且，他可以让您更*
>%%LINK%%[[#^4o7lgqnseoq|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#shell
^4o7lgqnseoq


>%%
>```annotation-json
>{"created":"2023-12-18T06:22:18.064Z","updated":"2023-12-18T06:22:18.064Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":500353,"end":500383},{"type":"TextQuoteSelector","exact":" Bourne Again SHell (简称  bash)","prefix":"  都各有其特点。至于  Linux  使用的这一种版本就称为『","suffix":" 』，这个  Shell  是  Bourne Shell  的"}]}]}
>```
>%%
>*%%PREFIX%%都各有其特点。至于  Linux  使用的这一种版本就称为『%%HIGHLIGHT%% ==Bourne Again SHell (简称  bash)== %%POSTFIX%%』，这个  Shell  是  Bourne Shell  的*
>%%LINK%%[[#^dgnqbczqawb|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #shell
^dgnqbczqawb


>%%
>```annotation-json
>{"created":"2023-12-18T06:26:48.224Z","text":"一些阉割部分功能的shell\n以限制用户的操作","updated":"2023-12-18T06:26:48.224Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":501442,"end":501461},{"type":"TextQuoteSelector","exact":"检查使用者能够使用的  shells ","prefix":"ells  这个文件啊？ 这是因为系统某些服务在运作过程中，会去","suffix":" ，而这些  shell  的查询就是藉由 /etc/shell"}]}]}
>```
>%%
>*%%PREFIX%%ells  这个文件啊？ 这是因为系统某些服务在运作过程中，会去%%HIGHLIGHT%% ==检查使用者能够使用的  shells== %%POSTFIX%%，而这些  shell  的查询就是藉由 /etc/shell*
>%%LINK%%[[#^9dbzgskarlf|show annotation]]
>%%COMMENT%%
>一些阉割部分功能的shell
>以限制用户的操作
>%%TAGS%%
>#shell
^9dbzgskarlf


>%%
>```annotation-json
>{"created":"2023-12-18T06:30:39.049Z","updated":"2023-12-18T06:30:39.049Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":502558,"end":502575},{"type":"TextQuoteSelector","exact":"命令编修能力  (history)","prefix":" shell  呢？  bash  主要的优点有底下几个：  ","suffix":"： bash  的功能里头，鸟哥个人认为相当棒的一个就是『他能记"}]}]}
>```
>%%
>*%%PREFIX%%shell  呢？  bash  主要的优点有底下几个： %%HIGHLIGHT%% ==命令编修能力  (history)== %%POSTFIX%%： bash  的功能里头，鸟哥个人认为相当棒的一个就是『他能记*
>%%LINK%%[[#^kxp9mztnqjk|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash
^kxp9mztnqjk


>%%
>```annotation-json
>{"created":"2023-12-18T06:31:43.131Z","updated":"2023-12-18T06:31:43.131Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":502752,"end":502765},{"type":"TextQuoteSelector","exact":".bash_history","prefix":"乎都被记录下来了。 这么多的指令记录在哪里呢？在你的家目录内的 ","suffix":" 啦！  不过，需要留意的是，~/.bash_history  "}]}]}
>```
>%%
>*%%PREFIX%%乎都被记录下来了。 这么多的指令记录在哪里呢？在你的家目录内的%%HIGHLIGHT%% ==.bash_history== %%POSTFIX%%啦！  不过，需要留意的是，~/.bash_history*
>%%LINK%%[[#^nkkep9crocs|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash
^nkkep9crocs


>%%
>```annotation-json
>{"created":"2023-12-18T06:32:15.319Z","updated":"2023-12-18T06:32:15.319Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":503091,"end":503100},{"type":"TextQuoteSelector","exact":"命令与文件补全功能","prefix":"目越多还是越少越好？这部份是见仁见智啦，没有一定的答案的。  ","suffix":"：  ([tab]  按键的好处) 还记得我们在第四章内的重要的"}]}]}
>```
>%%
>*%%PREFIX%%目越多还是越少越好？这部份是见仁见智啦，没有一定的答案的。 %%HIGHLIGHT%% ==命令与文件补全功能== %%POSTFIX%%：  ([tab]  按键的好处) 还记得我们在第四章内的重要的*
>%%LINK%%[[#^am9vyks0sb|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash
^am9vyks0sb


>%%
>```annotation-json
>{"created":"2023-12-18T06:33:14.103Z","updated":"2023-12-18T06:33:14.103Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":503565,"end":503583},{"type":"TextQuoteSelector","exact":"命令别名设定功能：  (alias)","prefix":"l  底下，多按几次  [tab]  是一个不错的习惯啦！  ","suffix":" 假如我需要知道这个目录底下的所有文件  (包含隐藏档)  及所"}]}]}
>```
>%%
>*%%PREFIX%%l  底下，多按几次  [tab]  是一个不错的习惯啦！ %%HIGHLIGHT%% ==命令别名设定功能：  (alias)== %%POSTFIX%%假如我需要知道这个目录底下的所有文件  (包含隐藏档)  及所*
>%%LINK%%[[#^llg1i7z87iq|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash
^llg1i7z87iq


>%%
>```annotation-json
>{"created":"2023-12-18T06:34:10.486Z","updated":"2023-12-18T06:34:10.486Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":504048,"end":504071},{"type":"TextQuoteSelector","exact":"程序化脚本：  (shell scripts)","prefix":"样的！此外，也可以在单一登录的环境中，达到多任务的目的呢！  ","suffix":" 在  DOS  年代还记得将一堆指令写在一起的所谓的『批处理文"}]}]}
>```
>%%
>*%%PREFIX%%样的！此外，也可以在单一登录的环境中，达到多任务的目的呢！ %%HIGHLIGHT%% ==程序化脚本：  (shell scripts)== %%POSTFIX%%在  DOS  年代还记得将一堆指令写在一起的所谓的『批处理文*
>%%LINK%%[[#^8dpqt37979|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash
^8dpqt37979


>%%
>```annotation-json
>{"created":"2023-12-18T06:34:28.866Z","updated":"2023-12-18T06:34:28.866Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":504185,"end":504190},{"type":"TextQuoteSelector","exact":"对谈交互式","prefix":"管理系统常需要下达的连续指令写成一个文件，  该文件并且可以透过","suffix":"的方式来进行主机的侦测工作！也可以藉由  shell  提供的环"}]}]}
>```
>%%
>*%%PREFIX%%管理系统常需要下达的连续指令写成一个文件，  该文件并且可以透过%%HIGHLIGHT%% ==对谈交互式== %%POSTFIX%%的方式来进行主机的侦测工作！也可以藉由  shell  提供的环*
>%%LINK%%[[#^mpmocsvcmj|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash
^mpmocsvcmj


>%%
>```annotation-json
>{"created":"2023-12-18T06:36:38.793Z","text":"*","updated":"2023-12-18T06:36:38.793Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":504377,"end":504394},{"type":"TextQuoteSelector","exact":"通配符：  (Wildcard) ","prefix":" 就可以帮你达成了！真的厉害！这部分我们在第十二章再来谈！  ","suffix":"除了完整的字符串之外，  bash  还支持许多的通配符来帮助用"}]}]}
>```
>%%
>*%%PREFIX%%就可以帮你达成了！真的厉害！这部分我们在第十二章再来谈！ %%HIGHLIGHT%% ==通配符：  (Wildcard)== %%POSTFIX%%除了完整的字符串之外，  bash  还支持许多的通配符来帮助用*
>%%LINK%%[[#^obglz215ftq|show annotation]]
>%%COMMENT%%
>*
>%%TAGS%%
>#bash
^obglz215ftq


>%%
>```annotation-json
>{"created":"2023-12-18T06:39:45.511Z","text":"内建指令","updated":"2023-12-18T06:39:45.511Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":504955,"end":505044},{"type":"TextQuoteSelector","exact":"方便  shell  的操作，其实  bash  已经『内建』了很多指令了，例如上面提到的  cd  ，  还有例如  umask  等等的指令，都是内建在  bash  当中的","prefix":"现的画面中，最上方竟然出现一堆指令的介绍？这是怎么回事？  为了","suffix":"呢！ 那我怎么知道这个指令是来自于外部指令(指的是其他非  ba"}]}]}
>```
>%%
>*%%PREFIX%%现的画面中，最上方竟然出现一堆指令的介绍？这是怎么回事？  为了%%HIGHLIGHT%% ==方便  shell  的操作，其实  bash  已经『内建』了很多指令了，例如上面提到的  cd  ，  还有例如  umask  等等的指令，都是内建在  bash  当中的== %%POSTFIX%%呢！ 那我怎么知道这个指令是来自于外部指令(指的是其他非  ba*
>%%LINK%%[[#^6y2g30lj2js|show annotation]]
>%%COMMENT%%
>内建指令
>%%TAGS%%
>#bash
^6y2g30lj2js


>%%
>```annotation-json
>{"created":"2023-12-18T06:42:08.165Z","text":"跳脱的意思是，让他后面那个键不进入这条命令的编写？所以对这条命令来说，就没有 Enter 来执行","updated":"2023-12-18T06:42:08.165Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":506438,"end":506500},{"type":"TextQuoteSelector","exact":" [Enter]  按键是紧接着反斜杠  (\\)  的，两者中间没有其他字符。  因为  \\  仅跳脱『紧接着的下一个字符』","prefix":"始执行』的功能！好让指令可以继续在下一行输入。 需要特别留意， ","suffix":"而已！所以，万一我写成： 『 \\ [Enter] 』，亦即  ["}]}]}
>```
>%%
>*%%PREFIX%%始执行』的功能！好让指令可以继续在下一行输入。 需要特别留意，%%HIGHLIGHT%% ==[Enter]  按键是紧接着反斜杠  (\)  的，两者中间没有其他字符。  因为  \  仅跳脱『紧接着的下一个字符』== %%POSTFIX%%而已！所以，万一我写成： 『 \ [Enter] 』，亦即  [*
>%%LINK%%[[#^t395ap9fvwh|show annotation]]
>%%COMMENT%%
>跳脱的意思是，让他后面那个键不进入这条命令的编写？所以对这条命令来说，就没有 Enter 来执行
>%%TAGS%%
>#bash
^t395ap9fvwh


>%%
>```annotation-json
>{"created":"2023-12-22T07:15:12.584Z","updated":"2023-12-22T07:15:12.584Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":508366,"end":508427},{"type":"TextQuoteSelector","exact":"不需要更动到程序代码啊！  只要将  MAIL  这个变量带入不同的内容即可让所有使用者透过  mail  取得自己的信件","prefix":"  mail  指令啊？反过来说，使用变量就变的很简单了！因为你","suffix":"！当然简单多了！  影响  bash  环境操作的变量 某些特"}]}]}
>```
>%%
>*%%PREFIX%%mail  指令啊？反过来说，使用变量就变的很简单了！因为你%%HIGHLIGHT%% ==不需要更动到程序代码啊！  只要将  MAIL  这个变量带入不同的内容即可让所有使用者透过  mail  取得自己的信件== %%POSTFIX%%！当然简单多了！  影响  bash  环境操作的变量 某些特*
>%%LINK%%[[#^xvvnd53q1fa|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#变量, #bash
^xvvnd53q1fa


>%%
>```annotation-json
>{"created":"2023-12-22T07:17:52.071Z","updated":"2023-12-22T07:17:52.071Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":508943,"end":509015},{"type":"TextQuoteSelector","exact":"这些环境变量例如  PATH、HOME、MAIL、SHELL  等等，都是很重要的，  为了区别与自定义变量的不同，环境变量通常以大写字符来表示","prefix":"的)  ，所以就有一些所谓的『环境变量』  需要来读入系统中了！","suffix":"呢！  脚本程序设计  (shell script)  的好帮"}]}]}
>```
>%%
>*%%PREFIX%%的)  ，所以就有一些所谓的『环境变量』  需要来读入系统中了！%%HIGHLIGHT%% ==这些环境变量例如  PATH、HOME、MAIL、SHELL  等等，都是很重要的，  为了区别与自定义变量的不同，环境变量通常以大写字符来表示== %%POSTFIX%%呢！  脚本程序设计  (shell script)  的好帮*
>%%LINK%%[[#^eqv8t569hh|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#变量, #bash
^eqv8t569hh


>%%
>```annotation-json
>{"created":"2023-12-22T07:18:59.544Z","text":"程序设计的思路","updated":"2023-12-22T07:18:59.544Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":509134,"end":509274},{"type":"TextQuoteSelector","exact":"该路径在  script  被使用在相当多的地方，如果下次换了一部主机，都要修改  script  里面的所有路径，那么我一定会疯掉！  这个时候如果使用变量，而将该变量的定义写在最前面，后面相关的路径名称都以变量来取代， 嘿嘿！那么你只要修改一行就等于修改整篇  script ","prefix":"有些数据因为可能由于用户习惯的不同而有差异，比如说路径好了，由于","suffix":" 了！方便的很！所以，良好的程序设计师都会善用变量的定义！  图"}]}]}
>```
>%%
>*%%PREFIX%%有些数据因为可能由于用户习惯的不同而有差异，比如说路径好了，由于%%HIGHLIGHT%% ==该路径在  script  被使用在相当多的地方，如果下次换了一部主机，都要修改  script  里面的所有路径，那么我一定会疯掉！  这个时候如果使用变量，而将该变量的定义写在最前面，后面相关的路径名称都以变量来取代， 嘿嘿！那么你只要修改一行就等于修改整篇  script== %%POSTFIX%%了！方便的很！所以，良好的程序设计师都会善用变量的定义！  图*
>%%LINK%%[[#^i46n6senq9m|show annotation]]
>%%COMMENT%%
>程序设计的思路
>%%TAGS%%
>#变量, #bash
^i46n6senq9m


>%%
>```annotation-json
>{"created":"2023-12-22T07:20:34.244Z","updated":"2023-12-22T07:20:34.244Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":509657,"end":509658},{"type":"TextQuoteSelector","exact":"$","prefix":"来取用变量，  但是，变量在被取用时，前面必须要加上钱字号『  ","suffix":"  』才行，举例来说，要知道  PATH  的内容，该如何是好？"}]}]}
>```
>%%
>*%%PREFIX%%来取用变量，  但是，变量在被取用时，前面必须要加上钱字号『%%HIGHLIGHT%% ==$== %%POSTFIX%%』才行，举例来说，要知道  PATH  的内容，该如何是好？*
>%%LINK%%[[#^8ivrpqm5ngx|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#变量, #bash
^8ivrpqm5ngx


>%%
>```annotation-json
>{"created":"2023-12-22T07:22:12.877Z","updated":"2023-12-22T07:22:12.877Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":509952,"end":509973},{"type":"TextQuoteSelector","exact":"加上  $  ，  或者是以  ${变量}","prefix":"面的范例，利用  echo  就能够读出，只是需要在变量名称前面","suffix":"  的方式来取用都可以！当然啦，那个  echo  的功能可是很"}]}]}
>```
>%%
>*%%PREFIX%%面的范例，利用  echo  就能够读出，只是需要在变量名称前面%%HIGHLIGHT%% ==加上  $  ，  或者是以  ${变量}== %%POSTFIX%%的方式来取用都可以！当然啦，那个  echo  的功能可是很*
>%%LINK%%[[#^cxw0z98kfls|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^cxw0z98kfls


>%%
>```annotation-json
>{"created":"2023-12-22T07:23:17.048Z","updated":"2023-12-22T07:23:17.048Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":510520,"end":510557},{"type":"TextQuoteSelector","exact":" 在  bash  当中，当一个变量名称尚未被设定时，预设的内容是『空』的","prefix":"Bird  这个数据啰～  而由上面的例子当中，我们也可以知道：","suffix":"。  另外，变量在设定时，还是需要符合某些规定的，否则会设定失败"}]}]}
>```
>%%
>*%%PREFIX%%Bird  这个数据啰～  而由上面的例子当中，我们也可以知道：%%HIGHLIGHT%% ==在  bash  当中，当一个变量名称尚未被设定时，预设的内容是『空』的== %%POSTFIX%%。  另外，变量在设定时，还是需要符合某些规定的，否则会设定失败*
>%%LINK%%[[#^3i6kc6mlmzg|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^3i6kc6mlmzg


>%%
>```annotation-json
>{"created":"2023-12-22T07:25:43.206Z","text":"可以来这参考","updated":"2023-12-22T07:25:43.206Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":510745,"end":510752},{"type":"TextQuoteSelector","exact":"变量的设定规则","prefix":"个不存在的变量，它是会出现错误讯息的喔！要注意！要注意！   ","suffix":" 1. 变量与变量内容以一个等号『=』来连结，如下所示：  『m"}]}]}
>```
>%%
>*%%PREFIX%%个不存在的变量，它是会出现错误讯息的喔！要注意！要注意！  %%HIGHLIGHT%% ==变量的设定规则== %%POSTFIX%%1. 变量与变量内容以一个等号『=』来连结，如下所示：  『m*
>%%LINK%%[[#^3l6xj0g1zn6|show annotation]]
>%%COMMENT%%
>可以来这参考
>%%TAGS%%
>#bash, #变量
^3l6xj0g1zn6


>%%
>```annotation-json
>{"created":"2023-12-22T07:27:32.319Z","text":"内容扩增\n有的话是累加，不会直接与之前的内容连起来。\n没有的话内容会连起来的","updated":"2023-12-22T07:27:32.319Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":511436,"end":511437},{"type":"TextQuoteSelector","exact":":","prefix":"或 ${变量} 累加内容，如下所示： 『PATH=\"$PATH\"","suffix":"/home/bin』或『PATH=${PATH}:/home/b"}]}]}
>```
>%%
>*%%PREFIX%%或 ${变量} 累加内容，如下所示： 『PATH="$PATH"%%HIGHLIGHT%% ==:== %%POSTFIX%%/home/bin』或『PATH=${PATH}:/home/b*
>%%LINK%%[[#^nj7374u7tsf|show annotation]]
>%%COMMENT%%
>内容扩增
>有的话是累加，不会直接与之前的内容连起来。
>没有的话内容会连起来的
>%%TAGS%%
>#bash, #变量
^nj7374u7tsf


>%%
>```annotation-json
>{"created":"2023-12-26T10:21:32.954Z","text":"作用域跟 C 语言是完全不一样的","updated":"2023-12-26T10:21:32.954Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":513337,"end":513402},{"type":"TextQuoteSelector","exact":"在一般的状态下，父程序的自定义变量是无法在子程序内使用的。但是透过 export  将变量变成环境变量后，就能够在子程序底下应用了","prefix":"个新的  shell  ，新的那个 shell  就是子程序啦！","suffix":"！很不赖吧！至于程序的相关概念，  我们会在第十六章程序管理当中"}]}]}
>```
>%%
>*%%PREFIX%%个新的  shell  ，新的那个 shell  就是子程序啦！%%HIGHLIGHT%% ==在一般的状态下，父程序的自定义变量是无法在子程序内使用的。但是透过 export  将变量变成环境变量后，就能够在子程序底下应用了== %%POSTFIX%%！很不赖吧！至于程序的相关概念，  我们会在第十六章程序管理当中*
>%%LINK%%[[#^skuen76rpz8|show annotation]]
>%%COMMENT%%
>作用域跟 C 语言是完全不一样的
>%%TAGS%%
>#bash, #变量
^skuen76rpz8


>%%
>```annotation-json
>{"created":"2023-12-26T10:24:13.607Z","text":"跟四则运算的规律比较像，先进行括号内的内容的运算","updated":"2023-12-26T10:24:13.607Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":511238,"end":511259},{"type":"TextQuoteSelector","exact":"使用反单引号『`指令`』或  『$(指令)","prefix":"在一串指令的执行中，还需要藉由其他额外的指令所提供的信息时，可以","suffix":"』。特别注意，那个 ` 是键盘上方的数字键 1 左边那个按键，而"}]}]}
>```
>%%
>*%%PREFIX%%在一串指令的执行中，还需要藉由其他额外的指令所提供的信息时，可以%%HIGHLIGHT%% ==使用反单引号『`指令`』或  『$(指令)== %%POSTFIX%%』。特别注意，那个 ` 是键盘上方的数字键 1 左边那个按键，而*
>%%LINK%%[[#^sw4mn6s8ff|show annotation]]
>%%COMMENT%%
>跟四则运算的规律比较像，先进行括号内的内容的运算
>%%TAGS%%
>#bash, #变量
^sw4mn6s8ff


>%%
>```annotation-json
>{"created":"2023-12-26T10:26:59.150Z","updated":"2023-12-26T10:26:59.150Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":514381,"end":514408},{"type":"TextQuoteSelector","exact":"双引号仍然可以保有变量的内容，但单引号内仅能是一般字符","prefix":"引号与双引号的用途有何不同？ 答： 单引号与双引号的最大不同在于","suffix":"  ，而不会有特殊符号。我们以底下的例子做说明：假设您定义了一个"}]}]}
>```
>%%
>*%%PREFIX%%引号与双引号的用途有何不同？ 答： 单引号与双引号的最大不同在于%%HIGHLIGHT%% ==双引号仍然可以保有变量的内容，但单引号内仅能是一般字符== %%POSTFIX%%，而不会有特殊符号。我们以底下的例子做说明：假设您定义了一个*
>%%LINK%%[[#^7p8fp1cw34g|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^7p8fp1cw34g


>%%
>```annotation-json
>{"created":"2023-12-26T10:28:53.651Z","text":"原如，平时工作时的小寄巧","updated":"2023-12-26T10:28:53.651Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":515267,"end":515331},{"type":"TextQuoteSelector","exact":"有一个常去的工作目录名称为：『/cluster/server/work/taiwan_2015/003/』，如何进行该目录的简化","prefix":" ls  指令来处理的意思啦！瞭了吗？  ^_^  例题： 若你","suffix":"？ 答： 在一般的情况下，如果你想要进入上述的目录得要『cd  "}]}]}
>```
>%%
>*%%PREFIX%%ls  指令来处理的意思啦！瞭了吗？  ^_^  例题： 若你%%HIGHLIGHT%% ==有一个常去的工作目录名称为：『/cluster/server/work/taiwan_2015/003/』，如何进行该目录的简化== %%POSTFIX%%？ 答： 在一般的情况下，如果你想要进入上述的目录得要『cd*
>%%LINK%%[[#^1t1cvknj0vi|show annotation]]
>%%COMMENT%%
>原如，平时工作时的小寄巧
>%%TAGS%%
>#bash, #变量
^1t1cvknj0vi


>%%
>```annotation-json
>{"created":"2023-12-26T10:44:56.023Z","updated":"2023-12-26T10:44:56.023Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":516961,"end":516990},{"type":"TextQuoteSelector","exact":"env  是  environment (环境)  的简写","prefix":"     <== 上一次使用的指令的最后一个参数(或指令本身) ","suffix":"啊，上面的例子当中，是列出来所有的环境变量。当然，如果使用 ex"}]}]}
>```
>%%
>*%%PREFIX%%<== 上一次使用的指令的最后一个参数(或指令本身)%%HIGHLIGHT%% ==env  是  environment (环境)  的简写== %%POSTFIX%%啊，上面的例子当中，是列出来所有的环境变量。当然，如果使用 ex*
>%%LINK%%[[#^bo28wmjty4w|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^bo28wmjty4w


>%%
>```annotation-json
>{"created":"2023-12-26T10:45:33.905Z","updated":"2023-12-26T10:45:33.905Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":517133,"end":517153},{"type":"TextQuoteSelector","exact":"家目录。还记得我们可以使用  cd ~ ","prefix":"功用呢？底下我们就一个一个来分析分析！  HOME 代表用户的","suffix":" 去到自己的家目录吗？或者利用  cd  就可以直接回到用户家目"}]}]}
>```
>%%
>*%%PREFIX%%功用呢？底下我们就一个一个来分析分析！  HOME 代表用户的%%HIGHLIGHT%% ==家目录。还记得我们可以使用  cd ~== %%POSTFIX%%去到自己的家目录吗？或者利用  cd  就可以直接回到用户家目*
>%%LINK%%[[#^rhq4u0fxtin|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^rhq4u0fxtin


>%%
>```annotation-json
>{"created":"2023-12-26T11:07:09.260Z","text":"感觉这个有问题啊","updated":"2023-12-26T11:07:09.260Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":518013,"end":518039},{"type":"TextQuoteSelector","exact":"number=$RANDOM*10/32768 ; ","prefix":"了： [dmtsai@study ~]$ declare -i ","suffix":"echo $number 8   <== 此时会随机取出 0~9"}]}]}
>```
>%%
>*%%PREFIX%%了： [dmtsai@study ~]$ declare -i%%HIGHLIGHT%% ==number=$RANDOM*10/32768 ;== %%POSTFIX%%echo $number 8   <== 此时会随机取出 0~9*
>%%LINK%%[[#^24hh9r2dw7x|show annotation]]
>%%COMMENT%%
>感觉这个有问题啊
>%%TAGS%%
>#bash, #变量
^24hh9r2dw7x


>%%
>```annotation-json
>{"created":"2023-12-26T11:08:24.631Z","text":"大概是这三种变量","updated":"2023-12-26T11:08:24.631Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":518155,"end":518208},{"type":"TextQuoteSelector","exact":"bash  可不只有环境变量喔，还有一些与  bash  操作接口有关的变量，以及用户自己定义的变量存在的","prefix":" 用  set  观察所有变量  (含环境变量与自定义变量) ","suffix":"。  那么这些变量如何观察呢？这个时候就得要使用  set  这"}]}]}
>```
>%%
>*%%PREFIX%% 用  set  观察所有变量  (含环境变量与自定义变量)%%HIGHLIGHT%% ==bash  可不只有环境变量喔，还有一些与  bash  操作接口有关的变量，以及用户自己定义的变量存在的== %%POSTFIX%%。  那么这些变量如何观察呢？这个时候就得要使用  set  这*
>%%LINK%%[[#^a8xwuuky2vb|show annotation]]
>%%COMMENT%%
>大概是这三种变量
>%%TAGS%%
>#bash, #变量
^a8xwuuky2vb


>%%
>```annotation-json
>{"created":"2023-12-26T11:09:30.052Z","updated":"2023-12-26T11:09:30.052Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":519441,"end":519486},{"type":"TextQuoteSelector","exact":"在  Linux  预设的情况中，使用{大写的字母}来设定的变量一般为系统内定需要的变量』","prefix":"口有关的变量，  通常都会被设定为大写字符，也就是说，『基本上，","suffix":"。  OK！OK！那么上头那些变量当中，有哪些是比较重要的？大概"}]}]}
>```
>%%
>*%%PREFIX%%口有关的变量，  通常都会被设定为大写字符，也就是说，『基本上，%%HIGHLIGHT%% ==在  Linux  预设的情况中，使用{大写的字母}来设定的变量一般为系统内定需要的变量』== %%POSTFIX%%。  OK！OK！那么上头那些变量当中，有哪些是比较重要的？大概*
>%%LINK%%[[#^8g8jvvy9qr|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^8g8jvvy9qr


>%%
>```annotation-json
>{"created":"2023-12-26T11:13:26.166Z","text":"命令提示符中所显示的内容","updated":"2023-12-26T11:13:26.166Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":520318,"end":520334},{"type":"TextQuoteSelector","exact":"『[\\u@\\h \\W]\\$  』","prefix":"了，让我们来看看  CentOS  预设的  PS1  内容吧：","suffix":"，现在你知道那些反斜杠后的数据意义了吧？  要注意喔！那个反斜杠"}]}]}
>```
>%%
>*%%PREFIX%%了，让我们来看看  CentOS  预设的  PS1  内容吧：%%HIGHLIGHT%% ==『[\u@\h \W]\$  』== %%POSTFIX%%，现在你知道那些反斜杠后的数据意义了吧？  要注意喔！那个反斜杠*
>%%LINK%%[[#^5it29dbaixq|show annotation]]
>%%COMMENT%%
>命令提示符中所显示的内容
>%%TAGS%%
>#bash, #变量
^5it29dbaixq


>%%
>```annotation-json
>{"created":"2023-12-26T11:15:00.882Z","updated":"2023-12-26T11:15:00.882Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":520791,"end":520836},{"type":"TextQuoteSelector","exact":"『目前这个  Shell  的线程代号』，亦即是所谓的  PID (Process ID)","prefix":"ll  的  PID) 钱字号本身也是个变量喔！这个咚咚代表的是","suffix":"。  更多的程序观念，我们会在第四篇的时候提及。想要知道我们的 "}]}]}
>```
>%%
>*%%PREFIX%%ll  的  PID) 钱字号本身也是个变量喔！这个咚咚代表的是%%HIGHLIGHT%% ==『目前这个  Shell  的线程代号』，亦即是所谓的  PID (Process ID)== %%POSTFIX%%。  更多的程序观念，我们会在第四篇的时候提及。想要知道我们的*
>%%LINK%%[[#^nrqhhs9vla9|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^nrqhhs9vla9


>%%
>```annotation-json
>{"created":"2023-12-26T11:15:57.793Z","text":"所以说 ？ 变量可以拿来查看错误代码？","updated":"2023-12-26T11:15:57.793Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":521037,"end":521139},{"type":"TextQuoteSelector","exact":"当我们执行某些指令时，  这些指令都会回传一个执行后的代码。一般来说，如果成功的执行该指令， 则会回传一个  0  值，如果执行过程发生错误，就会回传『错误代码』才对！一般就是以非为  0  的数值来取代","prefix":"值』，  上面这句话的重点是『上一个指令』与『回传值』两个地方。","suffix":"。  我们以底下的例子来看看： [dmtsai@study ~]"}]}]}
>```
>%%
>*%%PREFIX%%值』，  上面这句话的重点是『上一个指令』与『回传值』两个地方。%%HIGHLIGHT%% ==当我们执行某些指令时，  这些指令都会回传一个执行后的代码。一般来说，如果成功的执行该指令， 则会回传一个  0  值，如果执行过程发生错误，就会回传『错误代码』才对！一般就是以非为  0  的数值来取代== %%POSTFIX%%。  我们以底下的例子来看看： [dmtsai@study ~]*
>%%LINK%%[[#^4suebgh01t3|show annotation]]
>%%COMMENT%%
>所以说 ？ 变量可以拿来查看错误代码？
>%%TAGS%%
>#bash, #变量
^4suebgh01t3


>%%
>```annotation-json
>{"created":"2023-12-26T11:22:17.526Z","text":"硬件是基础，可以向下兼容，因为软件依靠硬件。","updated":"2023-12-26T11:22:17.526Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":522018,"end":522056},{"type":"TextQuoteSelector","exact":"较高阶的硬件通常会向下兼容旧有的软件，但较高阶的软件可能无法在旧机器上面安装","prefix":"86  兼容模式的安装光盘了～哇呜！进步的太快了！ 要留意的是，","suffix":"！  我们在第二章就曾说明过，  这里再强调一次，你可以在  x"}]}]}
>```
>%%
>*%%PREFIX%%86  兼容模式的安装光盘了～哇呜！进步的太快了！ 要留意的是，%%HIGHLIGHT%% ==较高阶的硬件通常会向下兼容旧有的软件，但较高阶的软件可能无法在旧机器上面安装== %%POSTFIX%%！  我们在第二章就曾说明过，  这里再强调一次，你可以在  x*
>%%LINK%%[[#^0hmiq78lusjc|show annotation]]
>%%COMMENT%%
>硬件是基础，可以向下兼容，因为软件依靠硬件。
>%%TAGS%%
>#bash, #变量
^0hmiq78lusjc


>%%
>```annotation-json
>{"created":"2023-12-26T11:23:13.652Z","text":"与 env 的区别就是会将环境变量以外的自定义变量也显示出来","updated":"2023-12-26T11:23:13.652Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":518247,"end":518287},{"type":"TextQuoteSelector","exact":"set  除了环境变量之外，  还会将其他在  bash  内的变量通通显示出来","prefix":"变量如何观察呢？这个时候就得要使用  set  这个指令了。  ","suffix":"哩！信息很多，底下鸟哥仅列出几个重要的内容： [dmtsai@s"}]}]}
>```
>%%
>*%%PREFIX%%变量如何观察呢？这个时候就得要使用  set  这个指令了。%%HIGHLIGHT%% ==set  除了环境变量之外，  还会将其他在  bash  内的变量通通显示出来== %%POSTFIX%%哩！信息很多，底下鸟哥仅列出几个重要的内容： [dmtsai@s*
>%%LINK%%[[#^jpm9uujy0a|show annotation]]
>%%COMMENT%%
>与 env 的区别就是会将环境变量以外的自定义变量也显示出来
>%%TAGS%%
>#bash, #变量
^jpm9uujy0a


>%%
>```annotation-json
>{"created":"2023-12-26T11:24:05.393Z","text":"跟编程语言里的环境变量的定义方式很不一样呢","updated":"2023-12-26T11:24:05.393Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":522252,"end":522278},{"type":"TextQuoteSelector","exact":"这两者的差异在于『 该变量是否会被子程序所继续引用』","prefix":"知道有所谓的环境变量与自定义变量，那么这两者之间有啥差异呢？其实","suffix":"啦！唔！那么啥是父程序？子程序？  这就得要了解一下指令的下达行"}]}]}
>```
>%%
>*%%PREFIX%%知道有所谓的环境变量与自定义变量，那么这两者之间有啥差异呢？其实%%HIGHLIGHT%% ==这两者的差异在于『 该变量是否会被子程序所继续引用』== %%POSTFIX%%啦！唔！那么啥是父程序？子程序？  这就得要了解一下指令的下达行*
>%%LINK%%[[#^zrkmennmc6q|show annotation]]
>%%COMMENT%%
>跟编程语言里的环境变量的定义方式很不一样呢
>%%TAGS%%
>#bash, #变量
^zrkmennmc6q


>%%
>```annotation-json
>{"created":"2023-12-26T11:30:14.511Z","updated":"2023-12-26T11:30:14.511Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":523004,"end":523026},{"type":"TextQuoteSelector","exact":"分享自己的变量设定给后来呼叫的文件或其他程序","prefix":"sai@study ~]$ export 变量名称 这东西用在『","suffix":"』啦！  像鸟哥常常在自己的主控文件后面呼叫其他附属文件(类似函"}]}]}
>```
>%%
>*%%PREFIX%%sai@study ~]$ export 变量名称 这东西用在『%%HIGHLIGHT%% ==分享自己的变量设定给后来呼叫的文件或其他程序== %%POSTFIX%%』啦！  像鸟哥常常在自己的主控文件后面呼叫其他附属文件(类似函*
>%%LINK%%[[#^s71048gzpog|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>#bash, #变量
^s71048gzpog


>%%
>```annotation-json
>{"created":"2023-12-26T11:32:22.127Z","text":"跟 env 一样","updated":"2023-12-26T11:32:22.127Z","document":{"title":"鸟哥的Linux私房菜-基础篇","link":[{"href":"urn:x-pdf:bfcee5792404759a96deda1a8a9256fe"},{"href":"vault:/Linux/Linux_Tutor.pdf"}],"documentFingerprint":"bfcee5792404759a96deda1a8a9256fe"},"uri":"vault:/Linux/Linux_Tutor.pdf","target":[{"source":"vault:/Linux/Linux_Tutor.pdf","selector":[{"type":"TextPositionSelector","start":523200,"end":523240},{"type":"TextQuoteSelector","exact":"仅下达  export  而没有接变量时，那么此时将会把所有的『环境变量』秀出来","prefix":"设定，这非常实用于  shell script  当中喔！ 如果","suffix":"喔！例如： [dmtsai@study ~]$ export d"}]}]}
>```
>%%
>*%%PREFIX%%设定，这非常实用于  shell script  当中喔！ 如果%%HIGHLIGHT%% ==仅下达  export  而没有接变量时，那么此时将会把所有的『环境变量』秀出来== %%POSTFIX%%喔！例如： [dmtsai@study ~]$ export d*
>%%LINK%%[[#^v6n1jten3y|show annotation]]
>%%COMMENT%%
>跟 env 一样
>%%TAGS%%
>#bash, #变量
^v6n1jten3y
