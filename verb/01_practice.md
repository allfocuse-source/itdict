收到！现在立刻开始**“大脑算法重构”专项训练**。

这些练习不是让你翻译，而是强迫你的眼球执行“结构解析”。请严格按照指令操作，不要纠结单词意思！

第一关：【真凶锁定】—— 找谓语动词

规则： 快速扫视，只找出每句话的核心主干动词（Main Verb）。忽略从句里的动词。

1.  The database administrator, who manages the entire server, provides access to the users.

      - 核心动词是： provides

2.  Commands entered into the terminal are executed immediately by the engine.

      - 核心动词是： executed

3.  To ensure data integrity, the system which runs on the cloud backs up files every hour.

      - 核心动词是： run

第二关：【视觉降噪】—— 括号过滤法

规则： 找出文中的“修饰语”（介词短语或从句），并用括号 ( ) 括起来，然后告诉我括号外面的主干是什么。

示例： The file (in the folder) is (empty). \to 主干：File is empty.

题目： The default configuration (of the PostgreSQL server) (located in the data directory) defines (how the system behaves).

  - 括号外的主干是： default configuration defines system 

第三关：【代码映射】—— 逻辑块识别

规则： 不要翻译成中文，请把这句话转换成**伪代码（Pseudo-code）**逻辑。

题目： Unless you specify a different port using the -p flag, the client will
attempt to connect to the default port 5432.

  - 逻辑映射：

if (default):
    port = 5432
else:
    port = different port

第四关：【逆向重组】—— 解决后置定语

规则： 英语喜欢把描述放后面，请你通过“先读后面”的方式，把下面这句拼成中文（不要逐词，要意群）。

题目： A tool [that provides a graphical interface] [for managing database objects]
[is available].

1.  块A：A tool (一个工具)
2.  块B：that provides a graphical interface (提供图形界面的)
3.  块C：for managing database objects (用来管理数据库对象的)
4.  块D：is available (是现成的/可用的)

  - 按中文语序组合（B+C+A+D）： 提供图形界面的一个工具是现成用来管理数据库对象的

请快速作答（可以直接发给我序号和答案），我来给你纠错。只有通过这种高强度的“找结构”训练，你的视觉高亮功能才能建立起来！
