# 翻译逻辑反转算法练习

这些练习不是让你背诵，而是让你在大脑里运行那个**“逻辑反转算法”**。

## 第一组：基础钩子练习（介词短语反转）
**规则：** 识别 `[钩子] + [目标]`，在翻译时将其反转为 `[目标] + [钩子]`。

1. **Source:** `in the database`
    - 逻辑拆解：[在...里] + [数据库]
    - 输出结果：________________（数据库里）
2. **Source:** `after login`
    - 逻辑拆解：[在...后] + [登录]
    - 输出结果：________________（登录后）
3. **Source:** `under the folder`
    - 逻辑拆解：[在...下] + [文件夹]
    - 输出结果：________________（文件夹下）

## 第二组：零件移位练习（状语挪位）
**规则：** 英语零件挂在屁股后面，中文零件要挪到动词前面。

1. **Source:** `I` (主) `work` (谓) `in the office` (地点零件).
    - 第一步（硬翻）：我 工作 在办公室。
    - 第二步（挪位）：我 **[在办公室]** 工作。
2. **Source:** `The system` (主) `runs` (谓) `at high speed` (方式零件).
    - 第一步（硬翻）：系统 运行 以高速。
    - 输出结果：________________（系统**[高速]**运行。）
3. **Source:** `We` (主) `start the meeting` (谓宾) `at 9 o'clock` (时间零件).
    - 第一步（硬翻）：我们 开始会议 在9点。
    - 输出结果：________________（我们**[在9点]**开始会议。）

## 第三组：后置补丁练习（定语从句反转）
**规则：** 看到 `that/which` 后面的长补丁，整体打包，提到名词前面加个“的”。

1. **Source:** `The bug` (名词) `[that you found yesterday]` (补丁).
    - 逻辑：那个Bug [你昨天发现的]。
    - 输出结果：________________（**[你昨天发现的]** 那个Bug。）
2. **Source:** `The file` (名词) `[which is on the desktop]` (补丁).
    - 逻辑：那个文件 [在桌面上的]。
    - 输出结果：________________（**[在桌面上的]** 那个文件。）
3. **Source:** `The user` (名词) `[who has no permission]` (补丁).
    - 逻辑：那个用户 [没有权限的]。
    - 输出结果：________________（**[没有权限的]** 那个用户。）

## 第四组：全系统解析（长难句 Debug）
**任务：** 请用“骨架不动，零件反转”的算法，解析下面这句 OA 系统开发中常见的需求。

**Source Code:**
`I` | `need to update` | `the permission list` | `in the OA system` | `after the meeting` | `which is held today`.

**Debug 步骤：**
1. **提取骨架（硬翻）：** 我需要更新权限列表...
2. **识别零件 A (方位)：** `in the OA system` → 在OA系统中
3. **识别零件 B (时间)：** `after the meeting` → 会议后
4. **识别零件 C (补丁)：** `which is held today` → 今天举行的（修饰会议）

**Final Output (重构后的中文)：**
____________________________________________________
（参考答案：我需要在**[今天举行的]** **[会议后]**，**[在OA系统中]** 更新权限列表。）

## 练习建议：
1. **不要追求文采**：只要逻辑是对的（零件位置放对了），就算成功。
2. **画线连接**：在练习时，学着画箭头，把屁股后面的零件往前指。
3. **反馈**：你可以试着回复第四组的答案，我帮你看看你的“解析器”运行得准不准！

**如果你准备好了，告诉我第四组你的解析结果。**

I found a bug in the code yesterday.
硬翻（试试看有没有毛病）：我找到一个BUG，在代码里，昨天
挪位（标准算法）：我昨天在代码里发现一个BUG

现在我们把难度再升一级，加上刚才说的 that 补丁（定语从句）。看看你的算法能不能跑通：
Source:
I | found | a bug | [that will crash the OA system] | in the code | yesterday.
提示：
骨架依然是：我发现一个BUG。
补丁：[that will crash the OA system]（会导致OA系统崩溃的）。这个补丁是修饰那个 BUG 的。
地点：in the code（在代码里）。
时间：yesterday（昨天）。

硬翻（看看多难受）： 我发现一个BUG，哪个会崩溃OA系统，在代码里，昨天
标准重构（最顺溜的中文）： 我昨天在代码里发现一个BUG，会导致OA系统崩溃
    “我昨天在代码里发现了一个**[会导致OA系统崩溃的]** BUG。”

Source:
The user | [who has no permission] | deleted | the file | [that contains financial data] | this morning.
提示：
骨架： 用户删除了文件。
补丁 1： [who has no permission] (没有权限的)，修饰“用户”。
补丁 2： [that contains financial data] (包含财务数据的)，修饰“文件”。
时间： this morning (今天早上)。
请开始你的算法表演：
你的重构版：用户在今天早上删除了没有权限的财务数据的文件
“那个**[没有权限的用户]，在[今天早上]，删除了那个[包含财务数据的文件]**。”

Source:
The manager | [of the IT department] | sent | an email | [about the new OA system] | to everyone.
提示：
骨架： 经理发了邮件给每个人。
补丁 1： [of the IT department] (IT部门的)，修饰谁？
补丁 2： [about the new OA system] (关于新OA系统的)，修饰谁？
你的重构版：经理发了关于新OA系统的邮件给IT部门的每个人
“[IT 部门的经理] 发了一封 [关于新 OA 系统的邮件] 给 [每个人]。”

Source:
The report | [on the table] | is | the file | [for the boss].
提示：
补丁 1： [on the table] (桌子上的)，紧跟在谁后面？
补丁 2： [for the boss] (给老板的)，紧跟在谁后面？
你的重构版： 桌子上的报告文件是给老板的
“[桌子上的报告] 是 [给老板的文件]。”
（别想业务，只看位置！看看桌子上的是“报告”还是“老板”！）

Source:
The programmer | [in our team] | is testing | the code | [for the OA system] | in the meeting room | now.
提示（按照邻居规则拆解）：
补丁 1： [in our team] (我们团队的)，修饰谁？
动作： is testing (正在测试)。
补丁 2： [for the OA system] (为了OA系统的/用于OA系统的)，修饰谁？
地点零件： in the meeting room (在会议室)。
时间零件： now (现在)。
请开始你的算法表演：
你的重构版：现在，我们团队的程序员，在会议室里，正在测试OA系统的代码
（注意：把“时间”和“地点”这两个大背景挪到动作前面，把“补丁”紧紧贴在它们的主人身上！）
