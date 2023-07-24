


# 标题（Headings）
创建标题需要在文字前面添加**井号 (`#`) 和空格(` `)**。井号的数量代表了标题的级别，井号越少级别越高。最多可以有六级标题。   


| Markdown 语法 | HTML | 渲染效果|
| ----------- | ----------- |----------- |
| # 标题1        |`<h1>标题1</h1>`|<h1>标题1</h1>|
| ## 标题2       |`<h2>标题2</h2>`|<h2>标题2</h2>|
| ### 标题3      |`<h3>标题3</h3>`|<h3>标题3</h3>|
| #### 标题4     |`<h4>标题4</h4>`|<h4>标题4</h4>|
| ##### 标题5    |`<h5>标题5</h5>`|<h5>标题5</h5>|
| ###### 标题6   |`<h6>标题6</h6>`|<h6>标题6</h6>|


(可选)还可在文本下方添加任意多的 == 号来标识一级标题，或者 -- 号来标识二级标题。

# 段落（Paragraph）
要创建段落，请使用空白行将一行或多行文本进行分隔。不要用空格（spaces）或制表符（ tabs）缩进段落。

# 换行（Line Break）
在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行(`<br>`)。

|Markdown 语法|HTML|渲染效果|
|---|---|---|
|第一行  &nbsp;&nbsp;<br>第二行|`<p>第一行  <br>`<br> `第二行</p>`|第一行  <br> 第二行|

为了兼容性，请在行尾添加“结尾空格”或 HTML 的 `<br>` 标签来实现换行。

# 强调（Emphasis）
通过将文本设置为粗体或斜体来强调其重要性。

## 粗体（Bold）
要加粗文本，请在需要加粗部分前后各添加两个星号（`**`）或下划线（`__`）。为了兼容性考虑，更推荐使用星号。

|Markdown语法|HTML|渲染效果|
|---|---|---|
|`我爱**粗体**.`|`我爱<strong>粗体</strong>.`|我爱**粗体**.|
|`我爱__粗体__.`|`我爱<strong>粗体</strong>.`|我爱**粗体**.|

## 斜体（Italic）
要用斜体显示文本，请在需要斜体显示的部分前后各添加一个星号（`*`）或下划线（`_`）。为了兼容性考虑，更推荐使用星号。

|Markdown语法|HTML|渲染效果|
|---|---|---|
|`我爱*斜体*.`|`我爱<em>斜体</em>.`|我爱*斜体*.|
|`我爱_斜体_.`|`我爱<em>斜体</em>.`|我爱*斜体*.|

## 粗体（Bold）和斜体（Italic）
要同时用粗体和斜体突出显示文本，请在需要强调的部分的前后各添加三个星号或下划线。或者混用星号和下划线。更推荐使用三个星号。

|Markdown语法|HTML|渲染效果|
|---|---|---|
|`这部分***非常重要***.`|`这部分<strong><em>非常重要</em></strong>.`|这部分**_非常重要_**.|
|`这部分___非常重要___.`|`这部分<strong><em>非常重要</em></strong>.`|这部分**_非常重要_**.|
|`这部分__*非常重要*__.`|`这部分<strong><em>非常重要</em></strong>.`|这部分**_非常重要_**.|
|`这部分**_非常重要_**.`|`这部分<strong><em>非常重要</em></strong>.`|这部分**_非常重要_**.|

## 删除线（Strikethrough）
可以用一条贯穿文本的横线表示删除某些文本。在文本前面和后面分别放置两个波浪号（`~~`） 来表示删除线。

```
~~世界是平坦的。~~ 我们现在知道世界是圆的。
```

~~世界是平坦的。~~ 我们现在知道世界是圆的。

# 引用（Quotes）
## 块引用（Blockquotes）
要创建块引用，请在段落前添加一个 `>` 符号。块引用可以包含多个段落。为段落之间的空白行添加一个 `>` 符号。（按Ctrl+Enter换行）

>当你排除了不可能的，无论剩下多么不可思议的，必然是真实的，不论多么不合乎常理。  
>
>逻辑只会带你到某处，而想象力将带你到任何地方。
>
>—— Sherlock Holmes

## 嵌套块引用（Nested Blockquotes）
块引用可以嵌套。在要嵌套的段落前添加一个 `>>` 符号。
>在阿瑟·柯南·道尔的《福尔摩斯探案集》中的故事《巴斯克维尔的猎犬》里，福尔摩斯向华生解释他对案件解决的推理过程时说到：
>>“当你排除了不可能的，无论剩下多么不可思议的，必然是真实的，不论多么不合乎常理。”

# 列表（Lists）
可以将多个条目组织成有序或无序列表。

## 有序列表 （Ordered List）
要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点再加上一个空格。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

|Markdown语法|HTML|编译效果|
|---|---|---|
|`1. First item ` <br>`2. Second item` <br>`3. Third item` <br>`4. Fourth item`|`<ol>` <br>`<li>First item</li>` <br>`<li>Second item</li>` <br>`<li>Third item</li>` <br>`<li>Fourth item</li>` <br>`</ol>`|1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item|

|有序列表各种写法1|写法2|写法3|预览效果|
|---|---|---|---|
|`1. First item ` <br>`2. Second item` <br>`3. Third item` <br>`4. Fourth item`|`1. First item ` <br>`1. Second item` <br>`1. Third item` <br>`1. Fourth item`|`1. First item ` <br>`8. Second item` <br>`3. Third item` <br>`5. Fourth item`|1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item|

还可以用Tab键（向后）和Shift+Tab键（向前）进行缩进来控制列表的级别。

1. First item
2. Second item
3. Third item
	1. Indented item1
	2. Indented item2
5. Fourth item

## 无序列表（Unordered Lists）
要创建无序列表，请在每个列表项前面添加破折号 (`-`)或星号 (`*`) 或加号 (`+`) 。缩进一个或多个列表项可创建嵌套列表。更推荐使用破折号(`-`)。

- First item
- Second item
- Third item
	- Indented item1
	- Indented item2
- Fourth item

如果需要以数字开头并且紧跟一个英文句号（也就是 `.`），则可以使使用反斜线（`\`）来转义这个英文句号。

# 代码
要将文本表示为代码，请将其包裹在反引号 (`` ` ``) 中。

## 转义反引号
如果要表示为代码的文本中包含一个或多个反引号，则需要将文本包裹在双反引号(` `` `)中。

|Markdown|HTML|渲染效果|
|---|---|---|
|``` ``Use `code` in your Markdown file.`` ```|``<code>Use `code` in your Markdown file.</code>``|``Use `code` in your Markdown file.``|

## 代码块（Code Blocks）
要创建代码块，将代码块的每一行缩进至少四个空格或一个制表符。

## 围栏代码块（fenced code blocks）
Markdown基本语法允许通过将行缩进四个空格或一个制表符来创建代码块，但是这样并不方便，可以使用围栏代码块将，在代码块之前和之后的行上使用三个反引号（`` ``` ``)或三个波浪号（`~~~`）。

可以在刚开始的三个反引号后面指定一种编程语言，从而显示语法高亮。


````
```python
print('Hello World!')
```
````

```python
print('Hello World!')
```

# 分割线
要创建分隔线，请在单独一行上使用三个或多个星号 (`***`)、破折号 (`---`) 或下划线 (`___`) ，并且不能包含其他内容。为了兼容性，最好在分隔线的前后均添加空白行。

---

# 链接（Links）
链接文本放在中括号内，链接地址放在后面的圆括号中，链接title可选。链接title是当鼠标悬停在链接上时会出现的文字，它放在圆括号中链接地址后面，用双引号包裹进来，跟链接地址之间以空格分隔。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

渲染效果如下：

这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。

对于网址和Email地址，使用尖括号`<>`可以很方便地把URL或者email地址变成可点击的链接。渲染效果如下：

<https://markdown.com.cn>

<shengquansu@qq.com>

# 图片（Images）
要添加图片，首先请添加感叹号（`!`），然后紧跟着是方括号，方括号中可添加替代文本（alt text，即图片显示失败后显示此文本），最后跟着圆括号，圆括号中添加图片资源的路径或 URL。你可以选择在圆括号中的 URL 之后添加标题（即 title 属性）。

```
![替代文本](图片路径或链接 "图片标题")
```

![沙漠巨石](https://ss2.meipian.me/users/1666185/59e820548c704f5c844d138a8d3fdc20.jpg?imageView2/2/w/750/h/1400/q/80 "大漠孤烟直，长河落日圆。")

# 转义字符（Escaping Characters）
要显示原本用于格式化 Markdown 文档的字符，在字符前面添加反斜杠字符 (`\`) 。
以下列出的字符都可以通过使用反斜杠字符从而达到转义目的。

|字符|名称|
|---|---|
|\\|反斜杠（backslash）|
| `|反引号 （backtick）(在代码块中显示反引号可将其包裹在双反引号中)|
|*|星号（asterisk）|
|_|下划线（underscore）|
|{ }|花括号（curly braces）|
|[ ]|方括号（brackets）|
|< >|angle brackets|
|( )|圆括号或括号（parentheses）|
|#|井号（pound sign）|
|+|加号（plus sign）|
|-|减号（minus sign） (也叫连字符 hyphen)|
|.|句点（dot）|
|!|感叹号（exclamation mark）|
|\||管道符（pipe） (在表格中显示管道符 (&#124;)可使用其HTML 字符编码（`&#124;`）)|

# HTML 内嵌标签
大多 Markdown 应用程序允许你在 Markdown 格式文本中添加 HTML 标签。

# 表格（Tables）

要添加表格，使用三个或多个连字符（`---`）创建每列的标题，并使用管道（`|`）分隔每列。可以选择在表的任一端添加管道。

```
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

呈现的输出如下所示：

|Syntax|Description|
|---|---|
|Header|Title|
|Paragraph|Text|

 使用连字符（hyphens）和管道符（pipes）创建表格会很乏味。若想要快速创建表格，使用 [Markdown 表格生成器](https://www.tablesgenerator.com/markdown_tables)。使用图形界面生成表格，然后将生成的 Markdown 格式的文本复制粘贴到文件中即可。

通过在标题行中的连字符（hyphens）的左侧或右侧或两侧添加冒号（`:`），可以将对应列中的文本向左或向右或居中对齐。

```
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

| Long Syntax      | Description | Test Long Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

# 任务列表（Task Lists）

任务列表（task lists 或者 checklists）是指创建带有复选框的项目列表。在任务列表项前面添加破折号（`-`）和中间带空格的方括号（`[ ]`）。要选中复选框，在方括号中间添加一个 `x` ，即（`[x]`）。

```
- [x] 学习Markdown语法
- [ ] 学习Obsidian使用方法
- [ ] 利用Obsidian构建知识网络
```

- [x] 学习Markdown语法
- [ ] 学习Obsidian使用方法
- [ ] 利用Obsidian构建知识网络

# Markdown语法速查表
[Markdown 速查表](https://markdown.com.cn/cheat-sheet.html)提供了所有 Markdown 语法元素的基本解释