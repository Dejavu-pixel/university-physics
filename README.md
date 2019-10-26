# 大学物理题解编写临时仓库
本仓库存放大学物理题解的$\mathrm{\LaTeX}$代码、插图等

## 排版者任务
- 自己敲代码，可以对原题解的解答格式进行修改，使尽量美观；
- 利用软件将电子版文件转成.tex 文档时，对不整齐的代码进行**整理简化**；

## 组织者任务
- 每次收上来以后及时排成完整的稿子。
- 反馈不足之处给编写者。

## 排版整体要求和细节规范
详见[学研部排版学习路线](https://qyxf.site/technique/typeset)

### 配图

- 配图需要尽量使用矢量格式的图片，推荐使用 Tikz 包进行绘制。
- 亦可使用 `\includegraphics` 插入点阵图片 (.png .jpg 格式)
- 配图不要采用照片，如必须采用，可以经过处理软件处理为黑白图片后插入文档中
- 配图需注明图名，标上序号。序号按照章节、题目序号分配。如：「Chp12_21」

### 选择题、填空题

- 题目与题目之间（代码）空两行
- 选择题解析中尽量使用行内公式 `$ Your Equation Here $`
- 请尽量使用中文标点
- 表示流程使用`$\rightarrow$`，表示“可以推出”用`$\Rightarrow$`。
- 填空题中，多个空的答案使用`\qquad`命令分隔

### 解答题

- 题目与题目之间空一行
- 解答题解析中公式部分使用行间公式 `$$ Your Equation Here $$`或`gather`环境等
- 等号需对齐的多行公式使用`align`或`aligned`等环境
- 用$\because$和$\therefore$的解答方式，让解答过程左对齐，等号对齐
- 解答题解析中不要将文字部分放到公式环境中

### 模板中的命令

- 所有题目需使用 `\exercise` `\solve ` 命令
注：我把模板里的`\solve`改了，整体占两个字符，保证首行缩进一致。
- 导数、微分等使用`\di`等命令（见.tex模板）

### 分数

- 无论使用`\dfrac`还是`\frac`，需保证分数与上下的行不能靠太近
- 分数作为分子分母的分数，用斜杠作为分数线。如：${{{{\left(\frac{V_A/p_A}{V_B/p_B}\right)}^{\gamma-1}}}}$

### 某些字体的使用

- 单位最好用正体，用`\mathrm{}`
- 数学符号一定要斜体，放在数学环境中
- 化学式请使用`\ce{化学式(formula)}`，添加`\usepackage[version=4]{mhchem}`宏包
- 罗马数字使用如下命令：`\newcommand{\RNum}[1]{\uppercase\expandafter{\romannumeral #1\relax}}`
- 下标尽量不用汉字；如果一定要用的话，字号不能太大；可以附带文字说明其含义。

### 定界符、限制符
- 括号、绝对值符号建议加上定界符`\left`,`\right`

## 需要完善的题目

- 可能有些解析不够细致
- 12.6，解答没有任何文字说明
- 11,12章有两个插图需要重画。