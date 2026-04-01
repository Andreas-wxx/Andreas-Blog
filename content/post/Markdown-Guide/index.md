---
title: "Markdown-Guide"
description: How to use Markdown
slug: "markdown-guide"
date: 2026-03-29T21:31:51+08:00
image: 
categories:
    - 指南
tags:
    - Markdown
weight: 1
---


# 一、标题

### <u>n个#+空格+标题内容</u>

>\# 一级标题
>
>\##二级标题

## 二级标题

#### ==快捷键：==

- ==Ctrl+数字1~6快速将选中的文本调成对应级别的标题==

- ==Ctrl+0可以快速将选中文本调成对应级别标题==

- ==Ctrl+加/减对标题级别进行加减==

	---

	

# 二、段落

### 1.换行

#### <u>除了直接“Enter”换行之外，还可以用“Shift+Enter”使得行间距更小（可通过启用源代码模式查看工作方式）</u>

### 2.分割线

#### <u>三个“-”或三个“*”后“Enter”即可</u>

---



# 三、文字显示

## 1.字体

### <u>粗体：用一对“**”括起来</u>

### <u>删除线：用一对“~~”括起来</u>

### <u>下划线：用“<u>  </u>”括起来</u>

### <u>斜体：用一对“*”括起来</u>

### <u>高亮：用一对“==”括起来</u>

==如果不想被识别成字体转换符，可在转换符前加“\”将转换符转义如：1\*2\*3==

==如果 \不想被识别成转义字符，在前面再加上一个\即可：2\\3==

> \*\*粗体\*\*
> \~\~删除线\~\~
> \<u>下划线\</u>
> \*斜体\*
> \==高亮==
> 黑体高亮下划线:\==\<u>\*\*  **\</u>==

##### 效果

**粗体**
~~删除线~~
<u>下划线</u>
*斜体*
==高亮==

==<u>**黑体高亮下划线**</u>==

#### ==快捷键==

- ==删除线：Shift+Alt+5==
- ==下划线：Ctrl+U==
- ==斜体：Ctrl+L==

## 2.上下标

### 1.上标

#### <u>将需要上标的内容用“^”括起来</u>

> x\^2\^
> x\^3\^+x\^2\^+x+1=0

##### 效果

x^2^
x^3^+x^2^+x+1=0

### 2.下标

#### <u>将需要下标的内容用“~”括起来</u>

```
H~2~O
CH~3~CH~2~CHO
```

##### 效果

H~2~O
CH~3~CH~2~CHO

---



# 四、列表

## 1.无序列表

### <u>”*“或“-”或“+”+空格</u>

##### 1.效果

- 仅仅
- 只有
- 一个
- 级别

##### 2.子类别

- 一级
	- 二级
		- 三级

#### ==快捷键：Ctrl+Shift+】==

## 2、有序列表

### <u>数字+“.”+空格</u>

##### 效果

1. 一标题
2. 二标题
	- 子内容
	- 内容二
3. 三标题

#### ==快捷键Ctrl+Shift+【==

==（使用Tab或Shift+Tab键进行标题级别转换）==

## 3、任务列表

### <u>”-“+空格+“[ ]”+空格（未完成）</u>

### <u>”-“+空格+“[x]”+空格（已完成）</u>

> \- [x] 油泵液压
>
> \- [ ] 滑油温度

##### 效果

- [x] 油泵液压
- [ ] 滑油温度

---



# 五、区块显示

### <u>“>”或“》”+空格</u>

> 外层区块
>
> > 内层区块
> >
> > > 最内层区块

---

# 六、代码显示

## 1、行内代码

#### <u>将代码用“ ` ”（英文输入法,位于Esc下方）括起来</u>

> \`int a=0;\`

##### 效果

`int a=0;`

#### ==快捷键：Ctrl+Shift+`==

## 2、代码块

#### <u>将代码块用三个“ `“括起来,或输入三个后按Enter</u>

> \```
>
> #include <stdio.h>
>
> int main()
>
> {
>
> printf(“Hello World”);
>
> return 0;
>
> }
>
> \```

##### 效果

```c
#include <stdio.h>
int main()
{
printf(“Hello World”);
return 0;
}
```

#### ==快捷键：Ctrl+Shift+K==

---



# 七、链接

#### <u>直接输入一个有效网址</u>

#### <u>[内容]（有效网址（http：//…））</u>==括号用英文输入法==

（为链接起名）

#### <u>[内容]（有效网址（http：//…）+“有效网址（http：//…）”）</u>

（指针移到上面时显示网址链接）

#### <u>链接到本文本只需将（）中内容换为所需连接到的标题即可</u>

（格式中#后不要加空格）

> www.baidu.com
>
> [百度]（http://www.baidu.com）
>
> [百度]（http://www.baidu.com”http://www.baidu.com“)
>
> [一、标题]（）

##### 效果

www.baidu.com
[百度](http://www.baidu.com)
[百度](http://www.baidu.com"http://www.baidu.com")
[一、标题](#一、标题)

#### ==快捷键：Ctrl+K==

---



# 八、脚注

（对文本进行解释说明，成对使用）

#### <u>“[\^…]“</u>

#### <u>“[\^…]“+“ ：”+对该文本的解释说明</u>

（如需多行编写，在需要分行文字前加上\<br>即可）

> “[\^①]“
>
> “[\^①]“:解释说明

##### 效果

三极管有c[^①],b[^②],e[^③]三个极

[^①]: Collector <br>集电极
[^②]:Base <br>基极
[^③]:emitter <br>发射极

---

# 九、图片插入

#### <u>“!”+[文字(可不输入)]+（图片路径“标题”）</u>

#### <u>右键图片可以完成一些图片操作</u>

##### <u>缩放：style="zoom: xx%;</u>

##### <u>对齐：align=“right/left”;</u>

<!-- > \!\[Bears队徽](C:\Users\hp\Pictures\E.F.Tarkov\549d22103c29896c69a507fc8e2a81d701eda5e3_raw.jpg) -->

##### 效果

<!-- <img src="C:\Users\hp\Pictures\E.F.Tarkov\549d22103c29896c69a507fc8e2a81d701eda5e3_raw.jpg" alt="Bears队徽" style="zoom: 25%;" /> -->

 

#### ==快捷键：Ctrl+Shift+i==

---



# 十、表格

### ==快捷键：Ctrl+T==

| 十进制 | 二进制 | 八进制 |
| ------ | ------ | ------ |
| 5      | 101    | 5      |
| 16     | 10000  | 20     |



---



# 十一、数学公式的插入

## 公式的插入

### 行中公式

#### <u>**将公式语句用“\$”括起来**</u>



### 独立公式（行间公式）

#### <u>**将公式语句用两个”\$$“括起来并Enter**</u>

效果
$$
y=ax^2
$$

## 上下标

#### 上标：用“^”引导上标内容

#### 下标：用“__”引导下标内容

代码

> x\^{12}\_1+x\^{35}\_2=3\^{2x}
>
> x\_1+x\_2=5

效果
$$
x^{12}_1+x^{35}_2=3^{2x}\\
x_1+x_2=5
$$

## 分数

#### <u>**使用函数“\frac{}{}”;“\dfrac{}{}”;“{}\over {}”**</u>

代码

> \\frac{a}{b}
>
> \dfrac{a}{b}
>
> {a}\over {b}

效果
$$
\frac{a}{b*\frac{c}{d}}\\
\dfrac{a}{b*\dfrac{c}{d}}\\
a\over{b*c\over d}
$$

## 开方

#### <u>**使用函数“\sqrt[根指数]{被开方数}”**</u>

==根指数省略时默认为二次方根==

代码

> \\sqrt{x}
>
> \sqrt[3z]{y}

效果
$$
\sqrt{2}\\
\sqrt[3z]{y}
$$

## 省略号

#### <u>**使用函数“\cdots”;“\ldots”;“\dots”;“\ddots”**</u>

效果

$\cdots\quad\ldots\quad\vdots\quad\ddots$

---

> 综合使用
>
> \$\frac{1}{\sqrt{n\^2+1}}+\frac{1}{\sqrt{n\^2+2}}+\\cdots+\frac{1}{\sqrt{n\^2+n}}$
> $$
> \frac{1}{\sqrt{n^2+1}}+\frac{1}{\sqrt{n^2+2}}+\cdots+\frac{1}{\sqrt{n^2+n}}
> $$
> 

---

## 矢量和均值

**将“\over”“\under”和“leftarrow”“rightarrow”“leftrightarrow”进行组合**
**来在内容上方或下方标箭头**

也可使用\vec{}对一个字母标上方右箭头

**使用“\overline”和“\underline”标上下横线**

代码

> \overrightarrow{a}
> \underleftarrow{G{vec{t}}}
> \overline{v}

$$
\overrightarrow{a}\\
\overleftarrow{G(\vec{t})}\\
\overline{v}
$$

## 积分符

#### <u>函数“\int”“\iint”\iiint</u>



代码

> \int{^2_3}
>
> \underset{D}\iint 或 \iint\limits_D
>
> \underset{\omega}\iiint 或 \iiint\limits_\omega

效果
$$
\int{^2_3}\\
\underset{D}\iint\\ 
\iint\limits_D\\
\underset{\omega}\iiint\\
\iiint\limits_\omega
$$

## 极限

#### <u>使用函数“\lim{}”</u>

\to :趋近于

\infin无穷（+\infin正无穷）

代码

> \lim\limits_{n\to\infin}{1+\frac{1}{x}}^n=e

效果

$\lim\limits_{n\to\infin}{1+\frac{1}{x}}^n=e$

## 希腊字母

<!-- ![image-20240906220717781](C:\Users\33657\AppData\Roaming\Typora\typora-user-images\image-20240906220717781.png) -->

## 其他字符

[Markdown 数学符号大全_markdown数学符号-CSDN博客](https://blog.csdn.net/oYinHeZhiGuang/article/details/119943358)

[Mathpix：AI 驱动的文档自动化](https://mathpix.com/)
