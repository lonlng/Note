# MarkDown For Typora

## 概述 -- Overview

```
varies--v.(大小、形状等)相异，不同，有别;(根据情况)变化，改变;变更;(略做)改变--vary的第三人称单数
vary--v.(大小、形状等)相异，不同，有别;(根据情况)变化，改变;变更;(略做)改变
GFM---GitHub Flavored Markdown
```

**MarkDown** 是由[Daring Fireball](http://daringfireball.net/)创建的;这个最初的指南准则地址在[这](http://daringfireball.net/projects/markdown/syntax)。但是，他的语法在不同的解析器和编辑器有所不同。**Typora**用的是 [GitHub][GFM]风格的**MarkDown**

- [MarkDown For Typora](#markdown-for-typora)
  - [概述 -- Overview](#%e6%a6%82%e8%bf%b0----overview)
  - [块元素 -- Block Elements](#%e5%9d%97%e5%85%83%e7%b4%a0----block-elements)
    - [段落和换行符 -- Paragraph and line breaks](#%e6%ae%b5%e8%90%bd%e5%92%8c%e6%8d%a2%e8%a1%8c%e7%ac%a6----paragraph-and-line-breaks)
    - [标题 -- Headers](#%e6%a0%87%e9%a2%98----headers)
    - [引号 -- Blockquotes](#%e5%bc%95%e5%8f%b7----blockquotes)
    - [列表 -- Lists](#%e5%88%97%e8%a1%a8----lists)
    - [任务列表 -- Task List](#%e4%bb%bb%e5%8a%a1%e5%88%97%e8%a1%a8----task-list)
    - [（围栏）代码块 -- (Fenced) Code Blocks](#%e5%9b%b4%e6%a0%8f%e4%bb%a3%e7%a0%81%e5%9d%97----fenced-code-blocks)
    - [数学块 -- Math Blocks](#%e6%95%b0%e5%ad%a6%e5%9d%97----math-blocks)
    - [表格 -- Tables](#%e8%a1%a8%e6%a0%bc----tables)
    - [注释 -- Fottnotes](#%e6%b3%a8%e9%87%8a----fottnotes)
    - [水平线 -- Horizontal Rules](#%e6%b0%b4%e5%b9%b3%e7%ba%bf----horizontal-rules)
    - [YAML Front Matter](#yaml-front-matter)
    - [目录 -- Tables of Contents(TOC)](#%e7%9b%ae%e5%bd%95----tables-of-contentstoc)
  - [行内元素 -- Span Elements](#%e8%a1%8c%e5%86%85%e5%85%83%e7%b4%a0----span-elements)
    - [链接 -- Links](#%e9%93%be%e6%8e%a5----links)
      - [内部链接 -- Internal Links](#%e5%86%85%e9%83%a8%e9%93%be%e6%8e%a5----internal-links)
      - [引用链接 -- Reference Links](#%e5%bc%95%e7%94%a8%e9%93%be%e6%8e%a5----reference-links)
    - [URLs](#urls)
    - [图片 -- Images](#%e5%9b%be%e7%89%87----images)
    - [Emphasis](#emphasis)
    - [字体加粗 -- Strong](#%e5%ad%97%e4%bd%93%e5%8a%a0%e7%b2%97----strong)
    - [代码 -- Code](#%e4%bb%a3%e7%a0%81----code)
    - [删除线 -- Strikethrough](#%e5%88%a0%e9%99%a4%e7%ba%bf----strikethrough)
    - [下划线 -- Underlines](#%e4%b8%8b%e5%88%92%e7%ba%bf----underlines)
    - [表情符号 -- Emoji :smile](#%e8%a1%a8%e6%83%85%e7%ac%a6%e5%8f%b7----emoji-smile)
    - [内联数学 -- Inline Math](#%e5%86%85%e8%81%94%e6%95%b0%e5%ad%a6----inline-math)
    - [下标 -- Subscript](#%e4%b8%8b%e6%a0%87----subscript)
    - [上标 -- Superscript](#%e4%b8%8a%e6%a0%87----superscript)
    - [字体高亮 -- Highlight](#%e5%ad%97%e4%bd%93%e9%ab%98%e4%ba%ae----highlight)
  - [HTML](#html)
    - [内容嵌套 -- Embed Contents](#%e5%86%85%e5%ae%b9%e5%b5%8c%e5%a5%97----embed-contents)
    - [视频 -- Video](#%e8%a7%86%e9%a2%91----video)
    - [其他HTML支持 -- Other HTML Support](#%e5%85%b6%e4%bb%96html%e6%94%af%e6%8c%81----other-html-support)

## 块元素 -- Block Elements

### 段落和换行符 -- Paragraph and line breaks

```
Paragraph and line breaks
Paragraph--n.段;段落--vt.将…分段;写短文报导
line breaks--换行符;   断行;  
consecutive--adj. 连续不断的;  
separated--adj. (和某人)分居的;  --v. (使)分开，分离;  分割;  划分;  (使)分离，分散;  隔开;  阻隔;  
separate的过去分词和过去式;
parsers--解析器;分析器;剖析器;解析;语法分析器
in order to为了;以便;目的在于; 要想……
recognize认识; 认出; 辨别出; 承认; 意识到; 认可，接受，赞成
leave离开; 离开居住地点; 遗弃; 丢弃; 假期; 休假; 准许; 许可
spaces空地，空间; 空; 空隙; 空子; 空当; 宽敞; 空旷; 开阔; 以一定间隔排列; space的第三人称单数和复数
at the end of在…末端; 在…的结尾
```

段落只是一行或多行连续的文本。在MarkDown源码中，段落之间用两行或多行空白隔开，在Typora中你仅仅需要一个空行（按一次`Return`）去创建一个新段落。
按`Shift`+`Return`去创建单个换行符。许多其他的解析器将会忽略单行分割符，所以为了使其他Markdown解析器识别你的换行符，你可以在行尾留两个空格符或者插入`<br>`。

### 标题 -- Headers

```
hash肉丁土豆; #号; 反复推敲; 仔细考虑; 把……弄糟; 斩碎; 斩; 剁; 细切
characters品质，性格; 特点，特性; 特点，特征，特色; 勇气; 毅力; character的第三人称单数和复数
line线; 线条; 界线; 场地线，场界; 皱纹; 褶子; 做衬里; 形成一层; 沿…形成行
header用头顶球; 头球; 标头，首标
levels数量，程度，浓度; 标准; 水平; 质量; 品级; 层次; 级别; 使平坦; 使平整; 摧毁，夷平; 使相等; 使平等; 使相似; level的第三人称单数和复数
For example例如;比如
input投入资源; 投入; 输入; 输入的信息; 输入端
followed by紧随其后;其次是
title名称，标题，题目; 一种，一本; 称号，头衔，职称，称谓; 加标题，定题目
content所容纳之物; 所含之物; 内容; 目录，目次; 主题，主要内容; 满意; 满足; 愿意; 知足; 使满意; 使满足
press报章杂志; 报刊; 印刷媒体; 记者; 新闻工作者; 新闻界; 报道; 评论; 压，挤，推，施加压力; 按，压; 将…塞进; 把…按入
Return回来; 回去; 返回; 带回; 送回; 放回; 退还; 恢复; 重现; 归来; 归还; 退回
key钥匙; 关键; 要诀; 键; 用键盘输入; 键入; 用钥匙划坏; 最重要的; 主要的; 关键的
will谈及将来; 愿，要，会，定要; 烦劳别人做事时用; 想要; 希望; 愿意; 喜欢; 立定志向; 决心; 决意; 立遗嘱将赠与; 立遗嘱赠与; 意志; 毅力; 自制力; 意愿; 心愿; 遗嘱
create创造; 创作; 创建; 造成，引起，产生; 授予; 册封
characters品质，性格; 特点，特性; 特点，特征，特色; 勇气; 毅力; character的第三人称单数和复数
block大块; 立方体; 大楼; 一栋楼房; 四面临街的一方块楼群; 街区; 堵塞; 阻塞; 堵住; 挡住; 妨碍; 阻碍
quoting引用; 引述; 举例说明; 开价; 出价; 报价; quote的现在分词
presented把…交给; 颁发; 授予; 提出; 提交; 展现，显示，表现; present的过去分词和过去式
inputting输入; input的现在分词
followed by紧随其后;其次是
generate产生; 引起
insert插入; 嵌入; 添加，加插; 插页，广告附加页; 插入物; 添加物
proper正确的; 恰当的; 符合规则的; 真正的; 像样的; 名副其实的; 符合习俗的; 正当的; 规矩的; 特定节日等用的仪式; 弥撒书的章节; 特赞
for you为了你; 为你; 给你
quotes引用; 引述; 举例说明; 开价; 出价; 报价; quote的第三人称单数和复数
Nested嵌套;嵌套的;套叠式;套叠
quote引用; 引述; 举例说明; 开价; 出价; 报价
inside在…内; 在…里; 少于; 在里面; 在监狱里; 被监禁; 里面; 内部; 内侧; 慢车道; 内侧，里道，内圈; 内部的; 里面的; 从内部了解到的; 内线干的
another又一; 再一; 另一; 不同的; 类似的
block大块; 立方体; 大楼; 一栋楼房; 四面临街的一方块楼群; 街区; 堵塞; 阻塞; 堵住; 挡住; 妨碍; 阻碍
adding增加; 加添; 加; 补充说; 继续说; add的现在分词
additional附加的; 额外的; 外加的
levels数量，程度，浓度; 标准; 水平; 质量; 品级; 层次; 级别; 使平坦; 使平整; 摧毁，夷平; 使
```

标题在行首使用1-6个哈希（`#`）字符，对应于报头级别1-6。例如：

``` markdown
# This is an H1   标题1

## This is an H2  标题2

###### This is an H6 标题6
```

在Typora中，输入`#`后跟标题内容，然后按`Return`键将创建标题

### 引号 -- Blockquotes

MarkDown使用邮件格式 > 字符进行块引用，它们表现为：

``` markdown
> This is a blockquote with two paragraphs. This is first paragraph.
>
> This is second pragraph. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.



> This is another blockquote with one paragraph. There is three empty line to seperate two blockquote.
```

在Typora中，输入`>`后跟你的引用内容将产生引用块，Typora将为您插入适当的`>`或换行符，嵌套的块引号（一个块引号在林一个块引号里），添加额外的`>`级别。

> 1
> >2
> >>3
> >>
> >>>4
> >>>
> >>>> 5

### 列表 -- Lists

```
input投入资源; 投入; 输入; 输入的信息; 输入端
item项目; 一件商品; 一则，一条
create创造; 创作; 创建; 造成，引起，产生; 授予; 册封
symbol象征; 符号; 代号; 记号; 用符号代表
replace with用…代替
ordered精心安排的; 组织有序的; 命令; 指挥; 要求; 订购; 订货; 要求提供服务; 点; order的过去分词和过去式
unordered--adj.无序的；无条理的
symbol象征; 符号; 代号; 记号; 用符号代表
source code源码
as follows如下;分别是
```

输入`* list item 1`将创建一个无序列表`*`符号可以替换为`+`或`-`。
输入`1. list item 1`将创建一个有序列表-它们的标记源代码如下：

``` markdown
## un-ordered list
*   Red
*   Green
*   Blue

## ordered list
1.  Red
2.  Green
3. Blue
```

### 任务列表 -- Task List

```
task任务，工作; 活动; 交给某人; 派给某人
lists一览表; 名单; 目录; 清单; 倾斜; 把…列表，列清单，拟订清单; 列举; 把…列入一览表; 列入销售清单，列入价目表; list的第三人称单数和复数
with和…在一起; 和; 同; 跟; 有; 具有; 带有; 用; 使用; 以; 借
items项目; 一件商品; 一则，一条; item的复数
marked显而易见的; 明显的; 显著的; 有标记成分的; 做记号; 做标记; 留下痕迹; 弄污; 使有污点; 标明方位; 标示; mark的过去分词和过去式
either任何一个; 每个，各方; 也; 而且; 要么…要么，不是…就是，或者…或者
incomplete不完整的; 不完全的; 不完善的; 未修毕，未完成
complete完全的，彻底的; 全部的; 完整的; 整个的; 包括，含有; 完成; 结束; 填写; 使完整; 使完美
For example例如;比如
change改变; 变化; 使不同; 变换，改换，变成; 变更; 变革; 替代; 更换; 替代物
complete完全的，彻底的; 全部的; 完整的; 整个的; 包括，含有; 完成; 结束; 填写; 使完整; 使完美
incomplete不完整的; 不完全的; 不完善的; 未修毕，未完成
state状态; 状况; 情况; 国家; 州; 邦; 国家提供的; 国事礼仪的; 州的; 邦的; 陈述; 说明; 声明; 规定; 公布
clicking使发出咔嗒声; 使咔嗒响; 点击，单击; 被突然明白; 豁然开朗; click的现在分词
checkbox复选框
before在…以前; 在…面前; 在前面; 到…为止; 到…之前; 以免; 不然; 以前; 过去; 已经
item项目; 一件商品; 一则，一条
```

任务列表是带有标记为[]或[x]的项（未完成或已完成）的列表。例如：

``` markdown
- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed
```

您可以通过单击项目前的复选框来更改完成/不完整状态。

- [ ] incomplete
- [x] completed

### （围栏）代码块 -- (Fenced) Code Blocks

```
only仅有的; 唯一的; 最好的; 最适当的; 只; 只有; 仅; 仅在…情况下; 只不过; 仅…而已; 不过; 但是; 可是
supports支持; 拥护; 鼓励; 帮助; 援助; 资助; 赞助; support的第三人称单数
fences栅栏; 篱笆; 围栏; 障碍物; 买卖赃物者; 销赃犯; 围住，隔开; 参加击剑运动; 搪塞; 支吾; 回避; fence的第三人称单数和复数
Original原来的; 起初的; 最早的; 首创的; 独创的; 有独创性的; 原作的; 真迹的; 非复制的; 原件; 正本; 原稿; 原作; 不同寻常的人，独特的人，怪人
code密码; 暗码; 电码; 代码; 编码; 道德准则; 行为规范; 为…编码; 把…译成密码; 编程序
blocks大块; 立方体; 大楼; 一栋楼房; 四面临街的一方块楼群; 街区; 堵塞; 阻塞; 堵住; 挡住; 妨碍; 阻碍; block的第三人称单数和复数
supported支持; 拥护; 鼓励; 帮助; 援助; 资助; 赞助; support的过去分词和过去式
fences栅栏; 篱笆; 围栏; 障碍物; 买卖赃物者; 销赃犯; 围住，隔开; 参加击剑运动; 搪塞; 支吾; 回避; fence的第三人称单数和复数
easy容易的; 轻易的; 不费力的; 舒适的; 安逸的; 安心的; 易受攻击的; 无自卫能力的; 容易吃亏的; 小心; 慢些; 轻点
Input投入资源; 投入; 输入; 输入的信息; 输入端
press报章杂志; 报刊; 印刷媒体; 记者; 新闻工作者; 新闻界; 报道; 评论; 压，挤，推，施加压力; 按，压; 将…塞进; 把…按入
return回来; 回去; 返回; 带回; 送回; 放回; 退还; 恢复; 重现; 归来; 归还; 退回
optional可选择的; 选修的
language语言; 语言文字; 言语; 说话; 某种类型的言语
identifier标识符，标识号，识别字
run跑; 奔跑; 跑步; 做跑步运动; 跑步的时间; 旅程，航程; 一段时光; 一系列
```

Typora只支持GitHub风格的标记。不支持标记中的原始代码块。

使用代码块很简单：输入\`\`\`并按`Return`。然后在\`\`\`后添加一个可选的语言标识符，我们将通过语法突出显示来运行它：

``` markdown
Here's an example:

​```
function test() {
  console.log("notice the blank line before this function?");
}
​```

syntax highlighting:
​```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
​```
```

### 数学块 -- Math Blocks

```
render使成为; 使变得; 使处于某状态; 给予; 提供; 回报; 递交; 呈献; 提交
using使用; 利用; 运用; 消耗; 说，写，使用; use的现在分词
mathematical--adj.数学的;(具有)数学(头脑)的;运算能力强的
expressions--n.表示;表达;表露;表情;神色;词语;措辞;表达方式-expression的复数
mathematical expression数学表达式
input投入资源; 投入; 输入; 输入的信息; 输入端
press报章杂志; 报刊; 印刷媒体; 记者; 新闻工作者; 新闻界; 报道; 评论; 压，挤，推，施加压力; 按，压; 将…塞进; 把…按入
Return回来; 回去; 返回; 带回; 送回; 放回; 退还; 恢复; 重现; 归来; 归还; 退回
trigger扳机; 起因，诱因; 触发器; 引爆器; 发动; 引起; 触发; 开动; 起动
accepts收受; 接受; 同意; 认可; accept的第三人称单数
For example例如;比如
field--n.田;地;牧场;(作某种用途的)场地;(覆盖…的或有…的)大片地方v.使参加竞选;使参加比赛;担任守队(队员);任守方;接，截，传(球)
math同 mathematics; 数学
block大块; 立方体; 大楼; 一栋楼房; 四面临街的一方块楼群; 街区; 堵塞; 阻塞; 堵住; 挡住; 妨碍; 阻碍
expression表示; 表达; 表露; 表情; 神色; 词语; 措辞; 表达方式
wrapped极高兴的; 十分满意的; 包，裹; 用…包裹; 用…缠绕; wrap的过去分词和过去式
a pair of一双
marks做记号; 做标记; 留下痕迹; 弄污; 使有污点; 标明方位; 标示; 污点; 污渍; 斑点; 疤痕; 斑点，色斑; 符号; 记号; 标记; mark的第三人称单数和复数
details细微之处; 枝节; 琐事; 详情; 全部细节; 具体情况; 资料，消息; 详细列举; 详细说明; 详述; 派遣; 选派; 分遣; 彻底清洗; detail的第三人称单数和复数
```

您可以使用**MathJax**呈现*LaTeX*数学表达式。

要添加数学表达式，请输入`$$`并按`Return`键。这将触发一个接受*Tex/LaTex*源的输入字段。例如：

$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$

在标记源文件中，数学块是由一对`$$`标记包装的*LaTeX*表达式：

``` markdown
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$
```

你可以在[这里](https://support.typora.io/Math/)找到更多的细节

### 表格 -- Tables

```
cloumns--n.柱;(通常为)圆形石柱;纪念柱;圆柱状物;柱形物;(书、报纸印刷页上的)栏--列
putting放; 安置; 猛推; 用力插入; 将…送往; 使…前往; put的现在分词; putt的现在分词
focus on关注，聚焦于
open up将开封; 拆开; 开放; 开通; 出现; 产生; 取得; 打开的门; 打开话匣子; 敞开心扉
toolbar工具栏
resize改变的大小
align排整齐; 校准; 使成一条直线; 使一致
delete删去; 删除
context背景，环境，来龙去脉; 上下文; 语境
columns柱; 圆形石柱; 纪念柱; 圆柱状物; 柱形物; 栏; column的复数
rows一排; 一列; 一行; 一排座位; 针行，一整行; 严重分歧; 纠纷; 吵架; 争吵; 大的噪音; 划; 划船送;
individual--adj.单独的;个别的;一个人的;供一人用的;独特的;与众不同的--n.个人;与众不同的人;有个性的人;某种类型的人;(尤指)古怪的人
syntax句法; 句法规则; 语构
tables桌子; 台子; 几; 一桌人; 表; 一览表; 提出，把…列入议事日程; 搁置; table的第三人称单数和复数
described描述; 形容; 把…称为; 做…运动; 画出…图形; 形成…形状; describe的过去分词和过去式
below在…下面; 少于; 低于; 在下面; 零度以下; 下级
necessary必需的; 必要的; 必然的; 无法避免的; 必需品
in detail详细地;全面地;仔细地
generated产生; 引起; generate的过去分词和过去式
automatically自动地；机械地；无意识地; 不经思索的
also而且; 此外; 也; 同样
include包括; 包含; 使成为…的一部分
inline一列式；排成行的；串联式的；联机的；轴向式的；在线上的
such as例如; 像; 象…这样; 诸如…之类
links联系; 连接; 关系; 纽带; 交通路线; 通讯手段; 把连接起来; 相关联; 说明有联系; link的第三人称单数和复数
bold大胆自信的; 敢于表白情感的; 敢于冒险的; 明显的; 轮廓突出的; 粗体的; 黑体的; 黑体; 粗体
italics斜体字; italic的复数
table桌子; 台子; 几; 一桌人; 表; 一览表; 提出，把…列入议事日程; 搁置
strikethrough--删除线;中划线;删除线效果;刪除線;加删除线
Finally终于; 最终; 最后; 彻底地; 决定性地
colons冒号; 结肠; colon的复数
within不出; 在之内; 在之间; 在里面; 在内部
define解释的含义; 给下定义; 阐明; 明确; 界定; 画出…的线条; 描出…的外形; 确定…的界线
text正文，本文; 文本; 文档; 演讲稿; 剧本; 文稿; 发短信
in that因为;原因是
colon冒号; 结肠
side一边，一侧; 一旁，一边; 侧面; 支持，偏袒
indicates表明; 显示; 象征; 暗示; 间接提及; 示意; indicate的第三人称单数
```

输入`| First Header  | Second Header |`然后按`Return`键，这将会创建一个包含两列的表格。

创建表后，将焦点放在该表上将打开该表的工具栏，您可以在其中调整、对齐或删除该表。也可以使用上下文菜单复制和添加/删除单个列/行。

表的完整语法如下所述，但不必详细了解完整语法，因为表的标记源代码是由Typora自动生成的。

在MarkDown源代码中，它们看起来像：、

``` markdown
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
```

还可以在表中包含内联标记，如链接、粗体、斜体或删除线。

最后，通过在标题行中包含冒号（`：`），可以将该列中的文本定义为左对齐、右对齐或居中对齐：

``` markdown
| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |
```

最左边的冒号表示左对齐的列；最右边的冒号表示右对齐的列；两边的冒号表示中间对齐的列。

### 注释 -- Fottnotes

```
footnotes脚注; 次要者; footnote的复数
like this像这样/像那样/照这样; 像这样
footnote脚注; 次要者
produce生产; 制造; 生长; 出产; 繁育; 制作，造出; 产品; 农产品
hover over停留于， 盘旋于; 威胁
footnote脚注; 次要者
superscript写在正常字符上方的; 标在上面的; 上角文字，上标
content所容纳之物; 所含之物; 内容; 目录，目次; 主题，主要内容; 满意; 满足; 愿意; 知足; 使满
content--n.所容纳之物;所含之物;内容;(书的)目录，目次;(书、讲话、节目等的)主题，主要内容--adj.满意;满足;愿意--v.满足;满意;知足;使满意;使满足
context--n.(事情发生的)背景，环境，来龙去脉;上下文;语境
```

``` markdown
You can create footnotes like this[^footnote].

[^footnote]: Here is the *text* of the **footnote**.
```

``` markdown
您可以创建这样的脚注[^footnote]。

[^footnote]: Here is the *text* of the **footnote**.
```

将产生：

您可以创建这样的脚注[^footnote]。

[^footnote]:这是**脚注**的*文本*。

将鼠标悬停在“脚注”上标上可查看脚注的内容。

### 水平线 -- Horizontal Rules

```
horizontal--adj.水平的;与地面平行的;横的--n.水平位置;水平线;水平面;横线;横切面
supports支持; 拥护; 鼓励; 帮助; 援助; 资助; 赞助; support的第三人称单数
at the top of在…最高地位; 用最高[最大]的
and then然后
introduce把…介绍; 引见; 介绍; 主持; 使初次了解; 使尝试
metadata元数据
alternatively要不，或者
article--n.(报刊上的)文章，论文，报道;(协议、契约的)条款，项;物件，物品(尤指整套中的一件)--vi.使受协议条款的约束;以协议（或契约）约束;订约将…收为学徒（或徒弟）;定约雇用进行控告;提出罪状（或指责）(against);签订协议
```

在空白的一行输入`***`或者`---`然后按`Return`键将会绘制一条水平线

### YAML Front Matter

```
matter--n.课题;事情;问题;事态;当前的状况;(询问某人的情况)怎么了--v.事关紧要;要紧;有重大影响
front--n.正面;前面;正前方;前部--adj.前面的;前部的;在前的;正面的;舌前位发的;舌前的--v.面向;在…前面;朝;向;用…作正面;用…覆盖正面;领导，代表(团体、组织等)
```

Typora现在支持[YAML Front Matter](http://jekyllrb.com/docs/frontmatter/)，在文章顶部输入`---`，然后按`Return`引入元数据块。或者，可以从Typora的顶部菜单插入元数据块。

### 目录 -- Tables of Contents(TOC)

```
section部分; 部门; 部件; 散件; 节; 款; 项; 段; 切开; 切断; 做切片; 强制入院治疗
extracts摘录; 选录; 选曲; 节录; 提取物; 浓缩物; 精; 汁; 提取; 提炼; 索取，设法得到; 选取; extract的第三人称单数和复数
headers用头顶球; 头球; 标头，首标; header的复数
document文件; 公文; 文献; 证件; 文档; 记录，记载; 用文件证明
contents所容纳之物; 所含之物; 内容; 目录，目次; 主题，主要内容; 满足; 满意; 知足; 使满意; 使满足; content的第三人称单数和复数
automatically自动地；机械地；无意识地; 不经思索的
add to增加，是对…的增添，加强
tables of contents 目录;目錄;目次;内容列表;内容目录
```

输入`[toc]`，然后按`Return`键。这将创建一个`目录`部分。目录从文档中提取所有标题，并且在您添加到文档时自动更新其内容。

## 行内元素 -- Span Elements

~~~
span--n.持续时间;范围;包括的种类;(桥或拱的)墩距，跨距，跨度--v.持续;贯穿;包括(广大地区);涵盖(多项内容);横跨;跨越
element--n.要素;基本部分;典型部分;少量;有点;有些;(大团体或社会中的)一组，一群，一伙
parsed作语法分析; 作句法分析; parse的过去分词和过去式
rendered使成为; 使变得; 使处于某状态; 给予; 提供; 回报; 递交; 呈献; 提交; render的过去分词和过去式
typing打字; 打字稿，文稿; 测定…的类型; 分型; 定型; type的现在分词
cursor光标，游标
explanation解释; 说明; 阐述; 解释性说法; 说明性文字
reference--n. 参考，参照；涉及，提及；参考书目；介绍信；证明书--vi. 引用--vt. 引用
expand--v.扩大，增加，增强(尺码、数量或重要性);扩展，发展(业务);细谈;详述;详细阐明
~~~

Span元素将在键入后立即解析和呈现。将光标移到这些跨元素的中间将把这些元素展开为标记源。下面是对每个span元素语法的解释。

### 链接 -- Links

```
delimited定…的界限; 限定; 界定; delimit的过去分词和过去式
square brackets -- 方括号;方括號;中括号;括弧;方括号内
square -- adj.正方形的;四方形的;成直角的;方的;(用于表示长度的单位后，表示某物四个边等长)…见方的--正方形;四方形;正方形物;(通常为方形的)广场;平方;二次幂--v.使成正方形;使成四方形;使成平方;使成二次幂;挺直身子;挺起胸膛--adv.正对着地;径直地
bracker--n.括号;(价格、年龄、收入等的)组级，等级;(固定在墙上的)托架，支架--v.用括弧括上;把…等同考虑;把…相提并论
inline一列式；排成行的；串联式的；联机的；轴向式的；在线上的
a set of一套; 一副
parentheses插入语; parenthesis的复数
closing接近尾声的，结尾的，结束的; 停业，关闭; 倒闭; 关; 关闭; 闭上; 合上; 合拢; 关门，关闭; 不开放; close的现在分词
square bracket方括号
link to将…连接起来；链接到
along with除某物以外; 随同…一起，跟…一起
surrounded围绕; 环绕; 包围，围住; 与…紧密相关; surround的过去分词和过去式
regular--adj.规则的;有规律的;间隙均匀的;定时的;频繁的;经常做(或发生)的;经常做某事的;常去某地的--n.常客;老主顾;主力(或正式)队员;(电视节目的)老主持人;经常参加某项活动的人;正规军人;职业军人
parentheses--n.插入语--parenthesis的复数---圆括号
parenthesis--n.插入语---括号
immediately--adv.立即;马上;即刻;接近;紧接;附近;紧接地;直接地--conj.一…就;即刻
point--n.论点;观点;见解;重点;要点;核心问题;意图;目的;理由--v.(用手指头或物体)指，指向;瞄准;对着;朝向
optional--adj.可选择的;选修的
quotes--v.引用;引述;举例说明;开价;出价;报价--n.引用v.引用;引述;举例说明;开价;出价;报价--n.引用
```

MarkDown支持两种链接样式：内联和引用。

在这两种样式中，链接文本由[方括号]分隔。

要创建内联链接，请在链接文本的右方括号后立即使用一组常规括号。在括号内，将链接指向的URL以及链接的可选标题放在引号中。例如：

``` markdown
This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.
```

将产生：

This is [an example](http://example.com/"Title") inline link. (`<p>This is <a href="http://example.com/" title="Title">`)

[This link](http://example.net/) has no title attribute. (`<p><a href="http://example.net/">This link</a> has no`)

#### 内部链接 -- Internal Links

```
internal--adj.内部的;里面的;体内的;(机构)内部的
set放; 置; 使处于; 使处于某种状况; 使开始; 把故事情节安排在; 以…为…设置背景; 一套，一副，一组; 一组; 一伙人; 阶层; 团伙; 位于…的; 安排好的; 确定的; 固定的; 顽固的; 固执的
href--horizontal reference 水平参考，水平基准
headers用头顶球; 头球; 标头，首标; header的复数
create创造; 创作; 创建; 造成，引起，产生; 授予; 册封
bookmark书签; 给…夹书签
allow允许; 准许; 给予; 允许进入
jump to猛增到jump to通常不用于进行体。
section部分; 部门; 部件; 散件; 节; 款; 项; 段; 切开; 切断; 做切片; 强制入院治疗
clicking使发出咔嗒声; 使咔嗒响; 点击，单击; 被突然明白; 豁然开朗; click的现在分词
For example例如;比如
Command命令; 指令; 控制; 管辖; 指挥; 指挥，统率; 应得; 博得; 值得
Ctrl计算机的Ctrl按键; 蹲; 按
jump to猛增到jump to通常不用于进行体。
header用头顶球; 头球; 标头，首标
cursor光标，游标
link with将…与…相连；连接在一起；与…联合
pressed紧缺，短绌; 压平的; 压扁的; 压，挤，推，施加压力; 按，压; 将…塞进; 把…按入; press的过去分词和过去式
element要素; 基本部分; 典型部分; 少量; 有点; 有些; 一组，一群，一伙
```

**您可以给标题设置一个href**，这将创建一个书签，允许您在单击后跳转到该部分。例如：

Command(on Windows: Ctrl) + Click [This link](#block-elements) will jump to header `Block Elements`. To see how to write that, please move cursor or click that link with `⌘` key pressed to expand the element into markdown source.

命令（在Windows上：Ctrl）+单击[此链接](#块元素 -- block elements)将跳转到标题`Block Elements`。若要查看如何编写，请移动光标或按“⌘”键单击该链接，将元素展开到标记源中。

#### 引用链接 -- Reference Links

```
reference--n.说到(或写到)的事;提到;谈及;涉及;参考;查询;查阅;(帮助或意见的)征求，征询--v.查阅;参考;给(书等)附参考资料
links联系; 连接; 关系; 纽带; 交通路线; 通讯手段; 把连接起来; 相关联; 说明有联系; link的第三人称单数和复数
second第二; 居第二位的; 另外的; 外加的; 以第二名; 以第二位; 第二，其次; 秒; 片刻; 瞬间; 支持，赞成; 附议; 临时调派; 短期调任
set of的; 集合; 释……的集合
inside在…内; 在…里; 少于; 在里面; 在监狱里; 被监禁; 里面; 内部; 内侧; 慢车道; 内侧，里道，内圈; 内部的; 里面的; 从内部了解到的; 内线干的
place位置; 地点; 场所; 地方; 城镇; 有某用途的建筑; 放置，安放; 使处于某位置; 安置; 安顿; 以某种态度对待
label标签; 签条; 标记; 称谓，绰号，叫法; 唱片公司; 贴标签于; 用标签标明; 把…称为
choosing选择; 挑选; 选取; 宁愿; 情愿; 决定; choose的现在分词
identify确认; 认出; 鉴定; 找到; 发现; 显示; 说明身份
link联系; 连接; 关系; 纽带; 交通路线; 通讯手段; 把连接起来; 相关联; 说明有联系
rendered--v.使成为;使变得;使处于某状态;给予;提供;回报;递交;呈献;提交--render的过去分词和过去式
render--v.使成为;使变得;使处于某状态;给予;提供;回报;递交;呈献;提交
implicit含蓄的; 不直接言明的; 成为一部分的; 内含的; 完全的; 无疑问的
shortcut近路;捷径; 快捷办法，捷径; 快捷方式
omit删除; 忽略; 漏掉; 遗漏; 不做; 未能做
name of【法】刑名
itself指施动并受其影响的动物或事物
for example例如;比如
web site网站
case--n.具体情况;事例;实例;实情;事实;特殊情况--v.奏爵士乐，跳爵士舞;游荡;使活泼
clicking使发出咔嗒声; 使咔嗒响; 点击，单击; 被突然明白; 豁然开朗; click的现在分词
link联系; 连接; 关系; 纽带; 交通路线; 通讯手段; 把连接起来; 相关联; 说明有联系
will谈及将来; 愿，要，会，定要; 烦劳别人做事时用; 想要; 希望; 愿意; 喜欢; 立定志向; 决心; 决意; 立遗嘱将赠与; 立遗嘱赠与; 意志; 毅力; 自制力; 意愿; 心愿; 遗嘱
expand扩大，增加，增强; 扩展，发展; 细谈; 详述; 详细阐明
editing编辑，校订; 编选; 编纂; 编集; 编辑; edit的现在分词
command命令; 指令; 控制; 管辖; 指挥; 指挥，统率; 应得; 博得; 值得
click使发出咔嗒声; 使咔嗒响; 点击，单击; 被突然明白; 豁然开朗; 短而尖的声音; 咔嗒声; 点按，单击; 吸气音
open开放的; 敞开的; 张开的; 张着的; 展开; 开放; 开; 打开; 开启; 户外; 野外; 旷野; 公开; 非秘密
hyperlink超级链接; 超链接; 把…做超级链接; 把…做超链接
```

引用链接使用第二组方括号，在其中放置选择的标签以标识链接：

``` markdown
This is [an example][id] reference-style link.

Then, anywhere in the document, you define your link label on a line by itself like this:

[id]: http://example.com/  "Optional Title Here"
```

在Typora中，它们的渲染方式如下：

这是[示例][id]引用样式链接。

[id]: http://example.com/ "Optional Title Here"

隐式链接名称快捷方式允许您省略链接的名称，在这种情况下，链接文本本身用作名称。只需使用一组空白的方括号-例如，要将“Google”链接到Google.com网站，您只需编写：

``` markdown
[Google][]
And then define the link:

[Google]: http://google.com/
```

在Typora中，单击链接将展开进行编辑，command+click将在您的web浏览器中打开超链接。

### URLs

```
allows允许; 准许; 给予; 允许进入; allow的第三人称单数
insert插入; 嵌入; 添加，加插; 插页，广告附加页; 插入物; 添加物
links联系; 连接; 关系; 纽带; 交通路线; 通讯手段; 把连接起来; 相关联; 说明有联系; link的第三人称单数和复数
wrapped极高兴的; 十分满意的; 包，裹; 用…包裹; 用…缠绕; wrap的过去分词和过去式
brackets括号; 组级，等级; 托架，支架; 用括弧括上; 把…等同考虑; 把…相提并论; bracket的第三人称单数和复数
also而且; 此外; 也; 同样
automatically自动地；机械地；无意识地; 不经思索的
link联系; 连接; 关系; 纽带; 交通路线; 通讯手段; 把连接起来; 相关联; 说明有联系
standard标准，水平，规格，规范; 正常的水平; 应达到的标准; 行为标准; 道德水准; 普通
Images【医】影象; 形象; 印象
similar相像的; 相仿的; 类似的; 类似物; 相像的人; 相似物
syntax句法; 句法规则; 语构
require需要; 依靠; 依赖; 使做; 使拥有; 规定
additional附加的; 额外的; 外加的
char烧黑，烧焦; 当家庭清洁工; 茶
start开始，着手，动手; 发生，开始进行; 开动; 发动; 启动; 开头; 开端; 开始; 起始优势; 良好的基础条件
inserting插入; 嵌入; 添加，加插; insert的现在分词
looks看; 瞧; 查找; 眼神; 表情; 神情; 脸色; 寻找; 寻求; 注意; 留心; 留神; look的第三人称单数和复数
like this像这样/像那样/照这样; 像这样
```

Typora允许您将URL作为链接插入，并用`<`括号`>`包装。

`<i@typora.io>` 变为 <i@typora.io>.

Typora还会自动链接标准URLs. e.g: www.google.com 。

### 图片 -- Images

```
Images【医】影象; 形象; 印象
similar相像的; 相仿的; 类似的; 类似物; 相像的人; 相似物
syntax句法; 句法规则; 语构
require需要; 依靠; 依赖; 使做; 使拥有; 规定
additional附加的; 额外的; 外加的
char烧黑，烧焦; 当家庭清洁工; 茶
start开始，着手，动手; 发生，开始进行; 开动; 发动; 启动; 开头; 开端; 开始; 起始优势; 良好的基础条件
inserting插入; 嵌入; 添加，加插; insert的现在分词
looks看; 瞧; 查找; 眼神; 表情; 神情; 脸色; 寻找; 寻求; 注意; 留心; 留神; look的第三人称单数和复数
like this像这样/像那样/照这样; 像这样
able to可以; 有能力; 原来能够按时完成
insert插入; 嵌入; 添加，加插; 插页，广告附加页; 插入物; 添加物
image file图像档案
source code源码
that is即; 用于纠正之前说过的内容
editing编辑，校订; 编选; 编纂; 编集; 编辑; edit的现在分词
able to可以; 有能力; 原来能够按时完成
drag拖，拉，拽，扯; 缓慢而费力地移动; 生拉硬拽; 劝勉强来; 令人厌烦的人; 乏味无聊的事; 累赘; 拖累; 绊脚石; 抽一口; 吸一口
insert插入; 嵌入; 添加，加插; 插页，广告附加页; 插入物; 添加物
image形象; 印象; 声誉; 画像; 雕像; 塑像; 反映; 想像; 作…的像; 象征
from从…起，始于; 从…开始; 寄自，得自
image file图像档案
drop--v.(意外地)落下，掉下，使落下;(故意)降下，使降落;累倒;累垮--n.滴;水珠;少量;微量;一点点;下降;下跌;减少
modify--v.调整;稍作修改;使更适合;缓和;使温和;修饰
relative--adj.相比较而言的;比较的;相对的;相关联的;相比之下存在(或有)的--n.亲戚;亲属;同类事物
currently--adv.现时;目前;当前;时下
editing--v.编辑，校订(文章、书籍等);编选;编纂;编集;(屏幕)编辑--edit的现在分词
sub-directory---子目录
specify具体说明; 明确规定; 详述; 详列
prefix前缀; 前置代号; 称谓; 在…前面加
and then然后
preview--n.预映;预演;预展;(报刊上有关电影、电视节目等的)预先评述，预告--v.为(影视节目)写预评;概述;扼要介绍
property--n.所有物;财产;财物;不动产;房地产;房屋及院落;庄园
treated--v.以…态度对待;以…方式对待;把…看作;把…视为;处理;讨论--treat的过去分词和过去式
treat--v.以…态度对待;以…方式对待;把…看作;把…视为;处理;讨论;治疗--n.乐事;乐趣;款待
```

图像的语法与链接相似，但它们需要额外的`!`链接开始前的字符。插入图像的语法如下：

``` markdown
![Alt text](/path/to/img.jpg)

![Alt text](/path/to/img.jpg "Optional title")
```

您可以使用拖放从图像文件或web浏览器插入图像。您可以通过单击图像来修改标记源代码。如果使用拖放添加的图像与当前编辑的文档位于同一目录或子目录中，则将使用相对路径。

如果您使用**MarkDown**来构建网站，则可以使用**YAML Front Matters**中的属性`typora-root-url`为本地计算机上的图像预览指定URL前缀。例如，在**YAML Front Matters**中输入`typora-root-url:/User/Abner/Website/typora.io/`，然后`![alt](/blog/img/test.png)`将被视为`![alt](file:///User/Abner/Website/typora.io/blog/img/test.png)`在Typora中。

您可以[在此处](https://support.typora.io/Images/)找到更多详细信息。

### Emphasis

```
emphasis--n.强调;重视;重要性;(对某个词或短语的)强调，加重语气，重读
treats以…态度对待; 以…方式对待; 把…看作; 把…视为; 处理; 讨论; 乐事; 乐趣; 款待; treat的第三人称单数和复数
asterisks星号; 加星号于; asterisk的第三人称单数和复数
underscores在…下面划线; 强调; 着重说明; 下划线，底线; underscore的第三人称单数和复数
indicators指示信号; 标志; 迹象; 指示器; 指针; 转向灯; 方向灯; indicator的复数
emphasis强调; 重视; 重要性; 强调，加重语气，重读
wrapped极高兴的; 十分满意的; 包，裹; 用…包裹; 用…缠绕; wrap的过去分词和过去式
tag标签; 标牌; 称呼; 诨名; 附加语(为加强语气，如Yes, I do一句中的I do); 给…加上标签;
E.g---例如
GFM---GitHub Flavored Markdown
ignore忽视; 对…不予理会; 佯装未见; 不予理睬
in words用…的话说;引用…的原话说
commonly通常; 常常; 大多数人地
code密码; 暗码; 电码; 代码; 编码; 道德准则; 行为规范; 为…编码; 把…译成密码; 编程序
like this像这样/像那样/照这样; 像这样
produce生产; 制造; 生长; 出产; 繁育; 制作，造出; 产品; 农产品
literal字面意义的; 完全按原文的; 缺乏想象力的
asterisk星号; 加星号于
underscore在…下面划线; 强调; 着重说明; 下划线，底线
position位置; 地方; 恰当位置; 正确位置; 姿态，姿势; 放置方式; 安装; 安置; 使处于
otherwise否则; 不然; 除此以外; 在其他方面; 另; 亦
delimiter定界符，分隔符
backslash反斜线
escape逃跑，逃走，逃出; 逃脱，摆脱，逃避; 避开，避免; 逃跑; 逃脱; 逃避; 逃避现实; 解脱;
recommends推荐; 举荐; 介绍; 劝告; 建议; 使显得吸引人; 使受欢迎; recommend的第三人称单数
symbol象征; 符号; 代号; 记号; 用符号代表
```

标记将星号（`*`）和下划线（`_`）视为强调的指示器。用一个`*`或`_`包装的文本将用一个HTML `<em>`标记包装。例如：

``` markdown
*single asterisks*

_single underscores_
```

输出显示:

*single asterisks*

_single underscores_

 [^GFM] 将忽略单词中的下划线，通常用于代码和名称，如下所示：

[^GFM]: GitHub Flavored Markdown.

> wow_great_stuff
>
> do_this_and_do_that_and_another_thing.

要在原本用作强调分隔符的位置生成文字星号或下划线，可以对其进行反斜杠转义：

``` markdown
\*this text is surrounded by literal asterisks\*
```

Typora建议使用`*`符号。

### 字体加粗 -- Strong

```
double两倍的; 加倍的; 双的; 成双的; 成对的; 供两者用的; 双人的; 双重地; 两倍地; 成对地; 弓身地; 两倍; 两倍数; 两倍量; 一杯双份的烈酒; 酷似的人; 极相似的对应物; 加倍; 是…的两倍; 把…对折; 折叠; 以二垒打使上二垒; 击出二垒安打
will谈及将来; 愿，要，会，定要; 烦劳别人做事时用; 想要; 希望; 愿意; 喜欢; 立定志向; 决心; 决意; 立遗嘱将赠与; 立遗嘱赠与; 意志; 毅力; 自制力; 意愿; 心愿; 遗嘱
cause原因; 起因; 理由; 动机; 缘故; 事业，目标，思想; 使发生; 造成; 引起; 导致
enclosed围住的，封闭的; 随函附上的; 附上的; 与外界隔绝的; 把…围起来; 围住; 附入; 随函附上; enclose的过去分词和过去式
contents所容纳之物; 所含之物; 内容; 目录，目次; 主题，主要内容; 满足; 满意; 知足; 使满意; 使满足; content的第三人称单数和复数
wrapped极高兴的; 十分满意的; 包，裹; 用…包裹; 用…缠绕; wrap的过去分词和过去式
HTML超文本标记语言
strong强壮的; 强健的; 强的; 强劲的; 强烈的，深刻的
tag标签; 标牌; 称呼; 诨名; 附加语(为加强语气，如Yes, I do一句中的I do); 给…加上标签; 把…
```

双`*`或`_`将使其包含的内容用HTML `<strong>`标记包装，例如：

``` markdown
**double asterisks**

__double underscores__
```

输出显示:

**double asterisks**

__double underscores__

Typora建议使用`**`符号

### 代码 -- Code

```
indicate表明; 显示; 象征; 暗示; 间接提及; 示意
inline一列式；排成行的；串联式的；联机的；轴向式的；在线上的
span持续时间; 范围; 包括的种类; 墩距，跨距，跨度; 持续; 贯穿; 包括; 涵盖; 横跨; 跨越
backtick---回音
quotes--v.引用;引述;举例说明;开价;出价;报价--n.引用
preformatted--预定义格式
wrap包，裹; 用…包裹; 用…缠绕; 披肩，围巾; 包裹材料; 完成拍摄，停机
quotes引用; 引述; 举例说明; 开价; 出价; 报价; quote的第三人称单数和复数
Unlike不像; 与…不同; 非…的特征; 不同; 相异
indicates表明; 显示; 象征; 暗示; 间接提及; 示意; indicate的第三人称单数
paragraph段; 段落; 将…分段; 写短文报导
For example例如;比如
```

要指示代码的内联范围，请用反引号（`）将其括起来。与预先格式化的代码块不同，代码范围指示正常段落中的代码。例如：

``` markdown
Use the `printf()` function.
```

显示结果:

Use the `printf()` function.

### 删除线 -- Strikethrough

```
strikethrough--删除线;加删除线;删除线效果
missing from在…中缺少的
```

GFM添加语法以创建删除线文本，标准**MarkDown**中缺少删除线文本。

`~~Mistaken text.~~` becomes ~~Mistaken text.~~

### 下划线 -- Underlines

```
underlines--v.在(词语等下)画线;画底线标出;强调;突现
powered---adj.由…驱动的;电动的--v.驱动，推动(机器或车辆);(使)迅猛移动，快速前进--power的过去分词和过去式
```

下划线是由原始HTML提供的。

`<u>Underline</u>` 变为 <u>Underline</u>.

### 表情符号 -- Emoji :smile

```
emoji表情符号
smile微笑; 笑; 微笑着说; 微笑地表示; 现出; 笑容
pressing紧急的; 急迫的; 难以推却的; 不容忽视的; 模压制品，同批次的模压产品; 压，挤，推，施加压力; 按，压; 将…塞进; 把…按入; press的现在分词
Council (United Nations))经济及社会理事会
enabling使能够; 使有机会; 使成为可能; 使可行; 使实现; enable的现在分词
preference偏爱; 爱好; 喜爱; 偏爱的事物; 最喜爱的东西
inputting输入; input的现在分词
Symbols象征; 符号; 代号; 记号; symbol的第三人称单数和复数
menu bar菜单栏
trigger扳机; 起因，诱因; 触发器; 引爆器; 发动; 引起; 触发; 开动; 起动
suggestions建议; 提议; 使人作推测的理由; 微量; 些微; 迹象; suggestion的复数
automatically自动地；机械地；无意识地; 不经思索的
panel嵌板，镶板，方格板块; 金属板，板金; 镶条，嵌条，饰片; 镶板
```

输入emoji，语法为`:smile:`。

用户可以按`ESC`键触发emoji的自动完成建议，或在“首选项”面板上启用后自动触发。此外，通过进入菜单栏（macOS）中的`Edit` -> `Emoji & Symbols`，还支持直接输入UTF-8表情符号字符。

### 内联数学 -- Inline Math

```
preference偏爱; 爱好; 喜爱; 偏爱的事物; 最喜爱的东西
Tab标签; 签条; 突耳; 凸舌; 账单，账款; 费用; 餐厅账单; 药片，药丸; 说适合于; 把视为…; 使用制表键
wrap包，裹; 用…包裹; 用…缠绕; 披肩，围巾; 包裹材料; 完成拍摄，停机
command命令; 指令; 控制; 管辖; 指挥; 指挥，统率; 应得; 博得; 值得
For example例如;比如
rendered使成为; 使变得; 使处于某状态; 给予; 提供; 回报; 递交; 呈献; 提交; render的过去
feature特色; 特征; 特点; 面容的一部分; 特写，专题节目; 以…为特色; 由…主演; 以…为主要组成; 起重要作用; 占重要地位
please请，请问; 请千万，请务必，的确; 太感谢了，太好了; 使满意; 使愉快; (常用在as或what、 where等词后)想，选择，喜欢
enable使能够; 使有机会; 使成为可能; 使可行; 使实现
trigger扳机; 起因，诱因; 触发器; 引爆器; 发动; 引起; 触发; 开动; 起动
inline一列式；排成行的；串联式的；联机的；轴向式的；在线上的
preview预映; 预演; 预展; 预先评述，预告; 为写预评; 概述; 扼要介绍
math同 mathematics; 数学
input投入资源; 投入; 输入; 输入的信息; 输入端
press报章杂志; 报刊; 印刷媒体; 记者; 新闻工作者; 新闻界; 报道; 评论; 压，挤，推，施加压力; 按，压; 将…塞进; 把…按入
ESC地球卫星公司(Earth Satellite Corporation); (=Economic and Social Council (United Nations))经济及社会理事会
key钥匙; 关键; 要诀; 键; 用键盘输入; 键入; 用钥匙划坏; 最重要的; 主要的; 关键的
command命令; 指令; 控制; 管辖; 指挥; 指挥，统率; 应得; 博得; 值得
```

若要使用此功能，请先在`Preference` 面板 -> `Markdown`选项卡中启用它。然后，使用`$`包装一个TeX命令。例如：`$\lim_{x \to \infty} \exp(-x) = 0$`将呈现为LaTeX命令。

显示结果：

---

$\lim_{x \to \infty} \exp(-x) = 0$

---

要触发内联数学的内联预览：输入`$`，然后按`ESC`键，然后输入一个TeX命令。

您可以在[此处](https://support.typora.io/Math/)找到更多详细信息。

### 下标 -- Subscript

```
feature特色; 特征; 特点; 面容的一部分; 特写，专题节目; 以…为特色; 由…主演; 以…为主要组成; 起重要作用; 占重要地位
enable使能够; 使有机会; 使成为可能; 使可行; 使实现
Preference偏爱; 爱好; 喜爱; 偏爱的事物; 最喜爱的东西
Panel嵌板，镶板，方格板块; 金属板，板金; 镶条，嵌条，饰片; 镶板
Tab标签; 签条; 突耳; 凸舌; 账单，账款; 费用; 餐厅账单; 药片，药丸; 说适合于; 把视为…; 使用制表键
wrap包，裹; 用…包裹; 用…缠绕; 披肩，围巾; 包裹材料; 完成拍摄，停机
subscript写在下面的; 下标
For example例如;比如
text正文，本文; 文本; 文档; 演讲稿; 剧本; 文稿; 发短信
```

若要使用此功能，请先在`Preference` 面板 -> `Markdown`选项卡中启用它。然后，使用`~`包装下标内容。例如：`H~2~O`, `X~long\ text~`/

### 上标 -- Superscript

```
Superscript--上標字;上标;上标字;上標;上角标
```

若要使用此功能，请先在`Preference` 面板 -> `Markdown`选项卡中启用它。然后，使用`^`包装上标内容。例如: `X^2^`.

### 字体高亮 -- Highlight

```
highlight--v.突出;强调;将(文本的某部分)用彩笔做标记;将(计算机屏幕的某区域)增强亮度;使醒目;挑染(将部分头发染成浅色)--n.最好(或最精彩、最激动人心)的部分;挑染的头发;(图画或照片的)强光部分
```

若要使用此功能，请先在`Preference` 面板 -> `Markdown`选项卡中启用它。然后，使用`==`包装突出显示内容。例如：`==highlight==`.

## HTML

```
HTML超文本标记语言
style方式; 作风; 样式; 款式; 时新，时髦，流行式样; 把…设计成某种式样; 称呼; 命名; 称
pure纯的; 纯净的; 纯粹的; 干净的; 不含有害物质的; 完全的
does not不; 不是; 否定就用
For example例如;比如
span持续时间; 范围; 包括的种类; 墩距，跨距，跨度; 持续; 贯穿; 包括; 涵盖; 横跨; 跨越
color彩色，颜色; 脸色，气色，肤色; 特色，个性；情调; 变红；脸红; 着色；渲染
text正文，本文; 文本; 文档; 演讲稿; 剧本; 文稿; 发短信
add增加; 加添; 加; 补充说; 继续说
```

您可以使用HTML来设置纯标记不支持的内容的样式。例如，使用`<span style="color:red">this text is red</span>`添加红色文本。

### 内容嵌套 -- Embed Contents

```
Some一些，若干; 某些，部分，有的; 好些; 不少的; 相当多的; 有些人，有些事物; 部分; 有的; 有些; 若干; (用于数词前，意同approximately)大约，差不多; 稍微; 有点
websites网站; website的复数
provide提供; 供应; 给予; 规定
embed把…牢牢地嵌入; 派遣; 嵌入(在I'm aware that she knows句中，she knows为内嵌句)
code密码; 暗码; 电码; 代码; 编码; 道德准则; 行为规范; 为…编码; 把…译成密码; 编程序
also而且; 此外; 也; 同样
For example例如;比如
```

有些网站提供基于`iframe`的嵌入代码，你也可以将其粘贴到Typora中。例如：

```Markdown
<iframe height='265' scrolling='no' title='Fancy Animated SVG Menu' src='http://codepen.io/jeangontijo/embed/OxVywj/?height=265&theme-id=0&default-tab=css,result&embed-version=2' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'></iframe>
```

### 视频 -- Video

```
video录像带; 盒式录像带; 录像，录影; 录像; 录电视节目; 给…录像
HTML超文本标记语言
tag标签; 标牌; 称呼; 诨名; 附加语(为加强语气，如Yes, I do一句中的I do); 给…加上标签; 把…称作; 给…起诨名; 加标识符于
embed把…牢牢地嵌入; 派遣; 嵌入(在I'm aware that she knows句中，she knows为内嵌句)
videos录像带; 盒式录像带; 录像，录影; 录像; 录电视节目; 给…录像; video的第三人称单数和复数
For example例如;比如
```

您可以使用`<video>`HTML标记嵌入视频。例如：

```Markdown
<video src="xxx.mp4" />
```

### 其他HTML支持 -- Other HTML Support

您可以在[此处](https://support.typora.io/HTML/)找到更多详细信息。

[GFM]: https://help.github.com/articles/github-flavored-markdown/
