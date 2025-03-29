# 公式编辑

- [概述](#概述)
    - [行内公式](#行内公式)
    - [行间公式](#行间公式)
    - [组](#组)
    - [自适应大小](#自适应大小)
- [希腊字母](#希腊字母)
- [占位符](#占位符)
- [括号](#括号)
- [上下标](#上下标)
- [比较](#比较)
- [代数](#代数)
    - [四则运算](#四则运算)
    - [高级运算](#高级运算)
    - [三角函数](#三角函数)
    - [无穷大](#无穷大)
    - [微积分](#微积分)
- [向量与矩阵](#向量与矩阵)
    - [向量](#向量)
    - [矩阵](#矩阵)
- [集合](#集合)
- [排列组合](#排列组合)
- [几何](#几何)
- [其他](#其他)
    - [省略号](#省略号)
    - [颜色](#颜色)

## 概述

一般公式分为两种形式，行内公式和行间公式

### 行内公式

在公式代码块的前后加上`$`，例如

$\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.$

``` 
$\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.$
```

### 行间公式

在公式代码块前后加上`$$` ，例如

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

``` 
$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$
```

### 组

单个字符或者使用`{}`包裹起来的内容，即一个组

### 自适应大小

在符号前加`\left`或`\right`，使符号大小与邻近的公式相适应

- 自适应前

    $(\sqrt{1 \over 2})^2$

    ```
    $(\sqrt{1 \over 2})^2$
    ```

- 自适应后

    $\left(\sqrt{1 \over 2}\right)^2$

    ```
    $\left(\sqrt{1 \over 2}\right)^2$
    ```

对于不显示的符号可以使用`.`代替

$\left. \frac{du}{dx} \right| _{x=0}$

```
$\left. \frac{du}{dx} \right| _{x=0}$
```

> 注：该语句适用于所有符号类型，但必须成对出现

## 希腊字母

|名称|大写|code|小写|code|
|:-:|:-:|:-:|:-:|:-:|
| alpha|A|A|α|\alpha|
| beta|B|B|β|\beta|

## 占位符

|类型|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|没空格||$xy$|&#36; xy &#36;| |
|小空格|\\,|$x\,y$|&#36; x \\, y &#36;|间距 3/18 em|
|中空格|\\:|$x\:y$|&#36; x \\: y &#36;|间距 4/18 em|
|大空格|\\ |$x\ y$|&#36; x \\  y &#36;|间距 5/18 em|
|长空格|\quad|$x \quad y$|&#36; x \quad y &#36;||
|两个长空格|\qquad|$x \qquad y$|&#36; x \qquad y &#36;||

> 注：暂时不知道大中小空格有啥区别

## 括号

|类型|左|右|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|:-:|
|圆括号|(|)|$(2+3)*x$|\$(2+3)*x\$| |
|方括号|[|]|$[2+3]*x$|\$[2+3]*x\$| |
|大括号|\\{|\\}|$\{a*b\}$|\$\{a*b\}\$|`{ }`用于分组|
|尖括号|\langle|\rangle|$\langle a*b \rangle$|\$\langle a*b \rangle\$|区分于小于号和大于号|

## 上下标

|类型|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|上标|^|$x^2$|\$x^2\$|
|下标|_|$x_i$|\$x_i\$|

> 注：上下标符号作用对象为一个组

## 比较

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|小于|\lt|$a \lt b$|\$a \lt b\$|
|大于|\gt|$a \gt b$|\$a \gt b\$|
|小于等于|\le|$a \le b$|\$a \le b\$|
|大于等于|\ge|$a \ge b$|\$a \ge b\$|
|等于|=|$a = b$|\$a = b\$|
|不等于|\ne|$a \ne b$|\$a \ne b\$|
|约等于|\approx|$a \approx b$|\$a \approx b\$|
|恒等于|\equiv|$a \equiv b$|\$a \equiv b\$|

> 注：以上符号前都可以加`\not`，例如 `$\not =$`表示$\not =$

## 代数

### 四则运算

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|加|+|$a+b$|\$a+b\$|
|减|-|$a-b$|\$a-b\$|
|乘|\times|$a \times b$|\$a \times b\$|
|点乘|· 或 \cdot|$a \cdot b$|\$a \cdot b\$|
|星乘|· 或 \ast|$a \ast b$|\$a \ast b\$|
|除|\div|$a \div b$|\$a \div b\$|
|斜除|/|$a / b$|\$a / b\$|
|加减|\pm|$a \pm b$|\$a \pm b\$|
|减加|\mp|$a \mp b$|\$a \mp b\$|
|绝对值|\lvert 和 \rvert|$\lvert x \rvert$|\$\lvert x \rvert\$|
|分数|\frac|$\frac {a}{b}$|\$\frac {a}{b}\$|
|分数|\over|${a} \over {b}$|\${a} \over {b}\$|
|模|\pmod|${a} \pmod {b}$|\${a} \pmod {b}\$|

### 高级运算

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|平均数|\overline|$\overline{abc}$|\$\overline{abc}\$|
|开方|\sqrt|$\sqrt {a+b}$|\$\sqrt {a+b}\$|
|开n次方|\sqrt[n]{m}|$\sqrt[3] {a+b}$|\$\sqrt[3] {a+b}\$|
|对数|\log|$\log(x)$|\$\log(x)\$|
|对数|\ln|$\ln(x)$|\$\ln(x)\$|以e为底|
|对数|\lg|$\lg(x)$|\$\lg(x)\$|以10为底|
|极限|\lim|$\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$|\$\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}\$|
|极限|\displaystyle \lim|$\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$|\$\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}\$|
|求和|\sum|$\sum_{i=1}^n$|\$\sum_{i=1}^n\$|
|求和|\displaystyle \sum|$\displaystyle \sum_{i=1}^n$|\$\displaystyle \sum_{i=1}^n\$|
|累乘|\prod|$\prod_{i=1}^{n}$|\$\prod_{i=1}^{n}\$|
|余积|\coprod|$\coprod_{i=1}^{n}$|\$\coprod_{i=1}^{n}\$|
|最大|\max|$\sum_{i=1}^n$|\$\sum_{i=1}^n\$|
|最小|\min|$\sum_{i=1}^n$|\$\sum_{i=1}^n\$|
|上取整|\lceil 和 \rceil|$\lceil x \rceil$|\$\lceil x \rceil\$|
|下取整|\lfloor 和 \rfloor|$\lfloor x \rfloor$|\$\lfloor x \rfloor\$|

### 三角函数

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|度|\circ|$45^\circ$|\$45^\circ\$|
|夹角|\angle|$\angle ACB$|\$\angle ACB\$|
|垂直|\bot|$L1 \bot L2$|\$L1 \bot L2\$|
|sin|\sin|$\sin(45^\circ)={{\sqrt 2} \over 2}$|\$\sin(45^\circ)={{\sqrt 2} \over 2}\$|
|cos|\cos|$\cos(45^\circ)={{\sqrt 2} \over 2}$|\$\cos(45^\circ)={{\sqrt 2} \over 2}\$|
|tan|\tan|$\tan(45^\circ)={1 \over 2}$|\$\tan(45^\circ)={1 \over 2}\$|
|cot|\cot|$\cot(45^\circ)={1 \over 2}$|\$\cot(45^\circ)={1 \over 2}\$|
|sec|\sec|$\sec(45^\circ)={1 \over 2}$|\$\sec(45^\circ)={1 \over 2}\$|
|csc|\csc|$\csc(45^\circ)={1 \over 2}$|\$\csc(45^\circ)={1 \over 2}\$|

### 无穷大

|运算符|符号|示例|
|:-:|:-:|:-:|
|无穷大|\infty|$\infty$|
|正无穷|+\infty|$+\infty$|
|负无穷|-\infty|$-\infty$|

### 微积分

- 微分

    |运算符|符号|示例|代码|
    |:-:|:-:|:-:|:-:|
    |微分|\partial|$\frac{\partial x}{\partial y}$|\$\frac{\partial x}{\partial y}\$|

- 积分

    |运算符|符号|示例|代码|
    |:-:|:-:|:-:|:-:|
    |积分|\int|$\int_{r=1}^\infty$|\$\int_{r=1}^\infty\$|
    |积分|\displaystyle \int|$\displaystyle \int_{r=1}^\infty$|\$\displaystyle \int_{r=1}^\infty\$|
    |双重积分|\iint|$\iint$|\$\iint\$|
    |三重积分|\iiint|$\iiint$|\$\iiint\$|

## 方程组 TODO

## 向量与矩阵

### 向量

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|向量|\vec|$\vec{a}$|\$\vec{a}\$||
|向量|\mathbf|$\mathbf{a}$|\$\mathbf{a}\$|粗体|

### 矩阵 TODO

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|积分|\int|$\int_{r=1}^\infty$|\$\int_{r=1}^\infty\$|

## 集合 TODO

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|属于|\in|$x \in y$|\$x \in y\$|
|不属于|\notin|$x \notin y$|\$x \notin y\$|
|交集|\cap|$A \cap B$|\$A \cap B\$|
|并集|\cup|$A \cup B$|\$A \cup B\$|
|差集|\setminus|$A \setminus B$|\$A \setminus B\$|

> 注：差集也可以直接用`-`号，即 `$A-B$`也表示差集 $A-B$

## 排列组合

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|排列|\binom {上位公式}{下位公式}|$\binom {n+1}{2k}$|\$\binom {n+1}{2k}\$|
|排列|{上位公式 \choose 下位公式}|${{n+1} \choose {2k}}$|\${{n+1} \choose {2k}}\$|
|组合|{上位公式 \atop 下位公式}|$\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots$|\$\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots\$|

## 几何 TODO

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|

## 其他

### 省略号

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|省略号|\dots|$\dots$|\$\dots\$|一般用于有下标的序列|
|省略号|\ldots|$\ldots$|\$\dots\$|
|省略号|\cdots|$\cdots$|\$\cdots\$|纵向位置比 \dots 稍高|
|省略号|\vdots|$\vdots$|\$\vdots\$|
|省略号|\ddots|$\ddots$|\$\ddots\$|

### 颜色

- 字体颜色

    ``` markdown
    ${\color{色调}表达式}$
    ```

- 背景颜色

    ```
    ${\pagecolor{色调}表达式}$
    ```

- 色调表

    |符号|示例|代码|
    |:-:|:-:|:-:|
    |Red|${\color{Red}Red}$|\${\color{Red}Red}\$|
    |Green|${\color{Green}Green}$|\${\color{Green}Green}\$|
    |Blue|${\color{Blue}Blue}$|\${\color{Blue}Blue}\$|
    |Yellow|${\color{Yellow}Yellow}$|\${\color{Yellow}Yellow}\$|
    |Orange|${\color{Orange}Orange}$|\${\color{Orange}Orange}\$|
    |Cyan|${\color{Cyan}Cyan}$|\${\color{Cyan}Cyan}\$|
    |Tan|${\color{Tan}Tan}$|\${\color{Tan}Tan}\$|
    |LimeGreen|${\color{LimeGreen}LimeGreen}$|\${\color{LimeGreen}LimeGreen}\$|
    |SpringGreen|${\color{SpringGreen}SpringGreen}$|\${\color{SpringGreen}SpringGreen}\$|
    |CornflowerBlue|${\color{CornflowerBlue}CornflowerBlue}$|\${\color{CornflowerBlue}CornflowerBlue}\$|
    |GreenYellow|${\color{GreenYellow}GreenYellow}$|\${\color{GreenYellow}GreenYellow}\$|