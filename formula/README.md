# 公式编辑

- [概述](#概述)
    - [行内公式](#行内公式)
    - [行间公式](#行间公式)
    - [换行](#换行)
    - [组](#组)
    - [自适应大小](#自适应大小)
    - [字体](#字体)
        - [文本字体](#文本字体)
        - [数学字体](#数学字体)
        - [其他字体](#其他字体)
        - [非标准命令](#非标准命令)
    - [颜色](#颜色)
        - [字体颜色](#字体颜色)
        - [背景颜色](#背景颜色)
        - [色调表](#色调表)
- [希腊字母](#希腊字母)
- [间距](#间距)
- [括号](#括号)
- [上下标](#上下标)
- [比较](#比较)
- [省略号](#省略号)
- [箭头](#箭头)
    - [定长箭头](#定长箭头)
    - [延伸箭头](#延伸箭头)
- [代数](#代数)
    - [四则运算](#四则运算)
    - [高级运算](#高级运算)
    - [三角函数](#三角函数)
    - [方程组](#方程组)
    - [分段函数](#分段函数)
    - [无穷大](#无穷大)
    - [微积分](#微积分)
    - [等号对齐](#等号对齐)
    - [其他符号](#其他符号)
- [向量](#向量)
- [矩阵](#矩阵)
    - [基础矩阵](#基础矩阵)
    - [省略元素](#省略元素)
    - [小矩阵](#小矩阵)
    - [增广矩阵](#增广矩阵)
    - [行列式](#行列式)
    - [矩阵范数](#矩阵范数) 
- [集合](#集合)
    - [符号](#符号)
    - [运算](#运算)
- [排列组合](#排列组合)

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

### 换行

在行尾加上 `\\` ，例如

$$
2x + 3y = 7 \\
5x - 2y = 2
$$

``` 
$$
2x + 3y = 7 \\
5x - 2y = 2
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

> [!NOTE]
> 该语句适用于所有符号类型，但必须成对出现

### 字体

#### 文本字体

||符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|---|
||\textup|$\textup{Ab0}$|&#36; \textup{Ab0} &#36;||
|文本字体|\textnormal|$\textnormal{Ab0}$|&#36; \textnormal{Ab0} &#36;|在​​数学模式中插入一段正常字体|
|罗马字体|\textrm|$\textrm{Ab0}$|&#36; \textrm{Ab0} &#36;|正体|
|粗体文本|\textbf|$\textbf{Ab0}$|&#36; \textbf{Ab0} &#36;||
|斜体文本|\textit|$\textit{Ab0}$|&#36; \textit{Ab0} &#36;||
|打字机字体|\texttt|$\texttt{Ab0}$|&#36; \texttt{Ab0} &#36;|等宽字体|
|无衬线字体|\textsf|$\textsf{Ab0}$|&#36; \textsf{Ab0} &#36;||
||\textmd|$\textmd{Ab0}$|&#36; \textmd{Ab0} &#36;||

#### 数学字体

||符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|---|
|数学斜体|\mathnormal|$\mathnormal{Ab0}$|&#36; \mathnormal{Ab0} &#36;|默认字体|
|罗马字体|\mathrm|$\mathrm{Ab0}$|&#36; \mathrm{Ab0} &#36;|正体|
|粗体|\mathbf|$\mathbf{Ab0}$|&#36; \mathbf{Ab0} &#36;||
|斜体|\mathit|$\mathit{Ab0}$|&#36; \mathit{Ab0} &#36;||
|花体|\mathcal|$\mathcal{Ab0}$|&#36; \mathcal{Ab0} &#36;|书法字体|
|黑板粗体|\mathbb|$\mathbb{Ab0}$|&#36; \mathbb{Ab0} &#36;|通常用于数集|
|弗兰克体|\mathfrak|$\mathfrak{Ab0}$|&#36; \mathfrak{Ab0} &#36;|哥特字体|
|打字机字体|\mathtt|$\mathtt{Ab0}$|&#36; \mathtt{Ab0} &#36;||
|无衬线字体|\mathsf|$\mathsf{Ab0}$|&#36; \mathsf{Ab0} &#36;||
|手写体|\mathscr|$\mathscr{Ab0}$|&#36; \mathscr{Ab0} &#36;|需要mathrsfs包|

#### 其他字体

||符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|---|
|粗体符号|\boldsymbol|$\boldsymbol{Ab0}$|&#36; \boldsymbol{Ab0} &#36;|用于希腊字母等|
|罗马字体|\rm|$\rm{Ab0}$|&#36; \rm{Ab0} &#36;|已弃用，用\mathrm代替|
|粗体|\bf|$\bf{Ab0}$|&#36; \bf{Ab0} &#36;|已弃用，用\mathbf代替|
|斜体|\it|$\it{Ab0}$|&#36; \it{Ab0} &#36;|已弃用，用\mathit代替|
|打字机字体|\tt|$\tt{Ab0}$|&#36; \tt{Ab0} &#36;|已弃用，用\mathtt代替|
|无衬线字体|\sf|$\sf{Ab0}$|&#36; \sf{Ab0} &#36;|已弃用，用\mathsf代替|

#### 非标准命令

||符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|---|
|粗体|\bold|$\bold{Ab0}$|&#36; \bold{Ab0} &#36;|等价于 \mathbf|
|花体|\cal|$\cal{Ab0}$|&#36; \cal{Ab0} &#36;|等价于 \mathcal|
|​​粗体符号|\bm|$\bm{Ab0}$|&#36; \bm{Ab0} &#36;|等价于 \boldsymbol|
|弗兰克体|\frak|$\frak{Ab0}$|&#36; \frak{Ab0} &#36;|等价于 \mathfrak|
|黑板粗体|\Bbb|$\Bbb{Ab0}$|&#36; \Bbb{Ab0} &#36;|等价于 \mathbb|

> [!IMPORTANT]  
> 非标准命令，可能在某些系统中不被支持

### 颜色

#### 字体颜色

||符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|---|
|文本颜色|\color{色调}{表达式}|$\color{Red}{a \times b}$|&#36; \color{Red}{a \times b} &#36;||
|文本颜色|\textcolor{色调}{表达式}|$\textcolor{Yellow}{a \div b}$|&#36; \textcolor{Yellow}{a \div b} &#36;||

#### 背景颜色

||符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|---|
|背景颜色|\colorbox{色调}{表达式}|$\colorbox{Orange}{a + b}$|&#36; \colorbox{Orange}{a + b} &#36;||
|背景颜色|\fcolorbox{色调}{aqua}{表达式}|$\fcolorbox{Orange}{aqua}{a - b}$|&#36; \colorbox{Orange}{aqua}{a - b} &#36;|反色|

#### 色调表

|符号|示例|代码|
|:-:|:-:|:-:|
|Red|${\color{Red}Red}$|&#36; {\color{Red}Red} &#36;|
|Green|${\color{Green}Green}$|&#36; {\color{Green}Green} &#36;|
|Blue|${\color{Blue}Blue}$|&#36; {\color{Blue}Blue} &#36;|
|Yellow|${\color{Yellow}Yellow}$|&#36; {\color{Yellow}Yellow} &#36;|
|Orange|${\color{Orange}Orange}$|&#36; {\color{Orange}Orange} &#36;|
|Cyan|${\color{Cyan}Cyan}$|&#36; {\color{Cyan}Cyan} &#36;|
|Tan|${\color{Tan}Tan}$|&#36; {\color{Tan}Tan} &#36;|
|LimeGreen|${\color{LimeGreen}LimeGreen}$|&#36; {\color{LimeGreen}LimeGreen} &#36;|
|SpringGreen|${\color{SpringGreen}SpringGreen}$|&#36; {\color{SpringGreen}SpringGreen} &#36;|
|CornflowerBlue|${\color{CornflowerBlue}CornflowerBlue}$|&#36; {\color{CornflowerBlue}CornflowerBlue} &#36;|
|GreenYellow|${\color{GreenYellow}GreenYellow}$|&#36; {\color{GreenYellow}GreenYellow} &#36;|
|#自定义颜色|${\color{#3399ff}{\#自定义颜色}}$|&#36; {\color{#3399ff}{#自定义颜色}} &#36;|

## 希腊字母

|    名称   |     大写    |    code  |    小写   |   code   |
| :-------: | :--------: | :------: | :-------: | :------: |
|  $alpha$  |    $A$     |    A     |  $\alpha$  |  \alpha  |
|  $beta$   |    $B$     |    B     |  $\beta$   |  \beta   |
|  $gamma$  |  $\Gamma$  |  \Gamma  |  $\gamma$  |  \gamma  |
|  $delta$  |  $\Delta$  |  \Delta  |  $\delta$  |  \delta  |
| $epsilon$ |    $E$     |    E     | $\epsilon$ | \epsilon |
|  $zeta$   |    $Z$     |    Z     |  $\zeta$   |  \zeta   |
|   $eta$   |    $H$     |    H     |   $\eta$   |   \eta   |
|  $theta$  |  $\Theta$  |  \Theta  |  $\theta$  |  \theta  |
|  $iota$   |    $I$     |    I     |  $\iota$   |  \iota   |
|  $kappa$  |    $K$     |    K     |  $\kappa$  |  \kappa  |
| $lambda$  | $\lambda$  | \lambda  | $\lambda$  | \lambda  |
|   $mu$    |    $M$     |    M     |   $\mu$    |   \mu    |
|   $nu$    |    $N$     |    N     |   $\nu$    |   \nu    |
|   $xi$    |   $\Xi$    |   \Xi    |   $\xi$    |   \xi    |
| $omicron$ |    $O$     |    O     | $\omicron$ | \omicron |
|   $pi$    |   $\Pi$    |   \Pi    |   $\pi$    |   \pi    |
|   $rho$   |    $P$     |    P     |   $\rho$   |   \rho   |
|  $sigma$  |  $\Sigma$  |  \Sigma  |  $\sigma$  |  \sigma  |
|   $tau$   |    $T$     |    T     |   $\tau$   |   \tau   |
| $upsilon$ | $\Upsilon$ | \Upsilon | $\upsilon$ | \upsilon |
|   $phi$   |   $\Phi$   |   \Phi   |   $\phi$   |   \phi   |
|   $chi$   |    $X$     |    X     |   $\chi$   |   \chi   |
|   $psi$   |   $\Psi$   |   \Psi   |   $\psi$   |   \psi   |
|  $omega$  |  $\Omega$  |  \Omega  |  $\omega$  |  \omega  |

## 间距

|类型|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|没间距||$xy$|&#36; xy &#36;| |
|小间距|\\,|$x \, y$|&#36; x \\, y &#36;|间距 3/18 em|
|小间距|\thinspace|$x \thinspace y$|&#36; x \thinspace y &#36;|间距 3/18 em|
|中间距|\\:|$x \: y$|&#36; x \\: y &#36;|间距 4/18 em|
|中间距|\medspace|$x \medspace y$|&#36; x \medspace y &#36;|间距 4/18 em|
|大间距|\\;|$x \; y$|&#36; x \\;  y &#36;|间距 5/18 em|
|大间距|\thickspace|$x \thickspace y$|&#36; x \thickspace  y &#36;|间距 5/18 em|
|长间距|\quad|$x \quad y$|&#36; x \quad y &#36;|间距 1 em|
|超长间距|\qquad|$x \qquad y$|&#36; x \qquad y &#36;|间距 2 em|
|不换行间距|~|$x ~ y$|&#36; x ~ y &#36;||
|小负间距|\negthinspace|$x \negthinspace y$|&#36; x \negthinspace y &#36;|间距 -3/18 em|
|中负间距|\negmedspace|$x \negmedspace y$|&#36; x \negmedspace y &#36;|间距 -4/18 em|
|大负间距|\negthickspace|$x \negthickspace y$|&#36; x \negthickspace  y &#36;|间距 -5/18 em|

## 括号

|类型|左|右|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|:-:|
|圆括号|(|)|$(2+3)*x$|&#36; (2+3)*x &#36;| |
|方括号|[|]|$[2+3]*x$|&#36; [2+3]*x &#36;| |
|大括号|\\{|\\}|$\{a*b\}$|&#36; \{a*b\} &#36;|`{ }`用于分组|
|尖括号|\langle|\rangle|$\langle a*b \rangle$|&#36; \langle a*b \rangle &#36;|区分于小于号和大于号|

## 上下标

|类型|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|上标|^|$x^2$|&#36; x^2 &#36;|
|下标|_|$x_i$|&#36; x_i &#36;|

> [!NOTE]  
> 上下标符号作用对象为一个**组**

## 比较

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|小于|\lt|$a \lt b$|&#36; a \lt b &#36;|
|大于|\gt|$a \gt b$|&#36; a \gt b &#36;|
|小于等于|\le|$a \le b$|&#36; a \le b &#36;|
|大于等于|\ge|$a \ge b$|&#36; a \ge b &#36;|
|等于|=|$a = b$|&#36; a = b &#36;|
|不等于|\ne|$a \ne b$|&#36; a \ne b &#36;|
|约等于|\approx|$a \approx b$|&#36; a \approx b &#36;|
|恒等于|\equiv|$a \equiv b$|&#36; a \equiv b &#36;|

> [!NOTE]  
> 以上符号前都可以加 `\not`，例如 `$\not =$` 表示 $\not =$

## 省略号

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|省略号|\dots|$\dots$|&#36; \dots &#36;|一般用于有下标的序列|
|省略号|\ldots|$\ldots$|&#36; \ldots &#36;||
|省略号|\cdots|$\cdots$|&#36; \cdots &#36;|纵向位置比 \dots 稍高|
|省略号|\vdots|$\vdots$|&#36; \vdots &#36;||
|省略号|\ddots|$\ddots$|&#36; \ddots &#36;||

## 箭头

### 定长箭头

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|上箭头|\uparrow|$\uparrow$|&#36; \uparrow &#36;||
|上箭头|\Uparrow|$\Uparrow$|&#36; \Uparrow &#36;||
|下箭头|\downarrow|$\downarrow$|&#36; \downarrow &#36;||
|下箭头|\Downarrow|$\Downarrow$|&#36; \Downarrow &#36;||
|上下箭头|\updownarrow|$\updownarrow$|&#36; \updownarrow &#36;||
|上下箭头|\Updownarrow|$\Updownarrow$|&#36; \Updownarrow &#36;||
|左箭头|\leftarrow|$\leftarrow$|&#36; \leftarrow &#36;||
|左箭头|\Leftarrow|$\Leftarrow$|&#36; \Leftarrow &#36;||
|左虚线箭头|\dashleftarrow|$\dashleftarrow$|&#36; \dashleftarrow &#36;||
|右箭头|\rightarrow|$\rightarrow$|&#36; \rightarrow &#36;||
|右箭头|\Rightarrow|$\Rightarrow$|&#36; \Rightarrow &#36;||
|右虚线箭头|\dashrightarrow|$\dashrightarrow$|&#36; \dashrightarrow &#36;||
|左右箭头|\leftrightarrow|$\leftrightarrow$|&#36; \leftrightarrow &#36;||
|左右箭头|\Leftrightarrow|$\Leftrightarrow$|&#36; \Leftrightarrow &#36;||
|左右长箭头|\longleftrightarrow|$\longleftrightarrow$|&#36; \longleftrightarrow &#36;||
|左右长箭头|\Longleftrightarrow|$\Longleftrightarrow$|&#36; \Longleftrightarrow &#36;||
|左右波浪箭头|\leftrightsquigarrow|$\leftrightsquigarrow$|&#36; \leftrightsquigarrow &#36;||
|上左下右箭头|\leftrightharpoons|$\leftrightharpoons$|&#36; \leftrightharpoons &#36;||
|上右下左箭头|\rightleftharpoons|$\rightleftharpoons$|&#36; \rightleftharpoons &#36;||
|斜上右箭头|\nearrow|$\nearrow$|&#36; \nearrow &#36;||
|斜上左箭头|\nwarrow|$\nwarrow$|&#36; \nwarrow &#36;||
|斜右下箭头|\searrow|$\searrow$|&#36; \searrow &#36;||
|斜左下箭头|\swarrow|$\swarrow$|&#36; \swarrow &#36;||
|左弯曲箭头|\curvearrowleft|$\curvearrowleft$|&#36; \curvearrowleft &#36;||
|右弯曲箭头|\curvearrowright|$\curvearrowright$|&#36; \curvearrowright &#36;||
|左循环箭头|\circlearrowleft|$\circlearrowleft$|&#36; \circlearrowleft &#36;||
|右循环箭头|\circlearrowright|$\circlearrowright$|&#36; \circlearrowright &#36;||

### 延伸箭头

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|左延伸箭头|\xleftarrow|$\xleftarrow{abc}$|&#36; \xleftarrow{abc} &#36;||
|左双延伸箭头|\xLeftarrow|$\xLeftarrow{abc}$|&#36; \xLeftarrow{abc} &#36;||
|右延伸箭头|\xrightarrow|$\xrightarrow{abc}$|&#36; \xrightarrow{abc} &#36;||
|右双延伸箭头|\xRightarrow|$\xRightarrow{abc}$|&#36; \xRightarrow{abc} &#36;||
|左右延伸箭头|\xleftrightarrow|$\xleftrightarrow{abc}$|&#36; \xleftrightarrow{abc} &#36;||
|左右双延伸箭头|\xLeftrightarrow|$\xLeftrightarrow{abc}$|&#36; \xLeftrightarrow{abc} &#36;||
|左上延伸箭头|\xleftharpoonup|$\xleftharpoonup{abc}$|&#36; \xleftharpoonup{abc} &#36;||
|左下延伸箭头|\xleftharpoondown|$\xleftharpoondown{abc}$|&#36; \xleftharpoondown{abc} &#36;||
|右上延伸箭头|\xrightharpoonup|$\xrightharpoonup{abc}$|&#36; \xrightharpoonup{abc} &#36;||
|右下延伸箭头|\xrightharpoondown|$\xrightharpoondown{abc}$|&#36; \xrightharpoondown{abc} &#36;||
|左右双向延伸箭头|\xtofrom|$\xtofrom{abc}$|&#36; \xtofrom{abc} &#36;||
|上左下右延伸箭头|\xleftrightharpoons|$\xleftrightharpoons{abc}$|&#36; \xleftrightharpoons{abc} &#36;||
|下左上右延伸箭头|\xrightleftharpoons|$\xrightleftharpoons{abc}$|&#36; \xrightleftharpoons{abc} &#36;||
|左映射延伸箭头|\xmapsto|$\xmapsto{abc}$|&#36; \xmapsto{abc} &#36;||
|左右等长延伸箭头|\xlongequal|$\xlongequal{abc}$|&#36; \xlongequal{abc} &#36;||

## 代数

### 四则运算

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|加|+|$a+b$|&#36; a+b &#36;|
|减|-|$a-b$|&#36; a-b &#36;|
|乘|\times|$a \times b$|&#36; a \times b &#36;|
|点乘|· 或 \cdot|$a \cdot b$|&#36; a \cdot b &#36;|
|星乘|· 或 \ast|$a \ast b$|&#36; a \ast b &#36;|
|除|\div|$a \div b$|&#36; a \div b &#36;|
|斜除|/|$a / b$|&#36; a / b &#36;|
|整除|\mid|$a \mid b$|&#36; a \mid b &#36;|
|加减|\pm|$a \pm b$|&#36; a \pm b &#36;|
|减加|\mp|$a \mp b$|&#36; a \mp b &#36;|
|绝对值|\lvert 和 \rvert|$\lvert x \rvert$|&#36; \lvert x \rvert &#36;|
|分数|\frac|$\frac {a}{b}$|&#36; \frac {a}{b} &#36;|
|分数|\over|${a} \over {b}$|&#36; {a} \over {b} &#36;|
|模|\pmod|${a} \pmod {b}$|&#36; {a} \pmod {b} &#36;|

### 高级运算

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|平均数|\overline|$\overline{abc}$|&#36; \overline{abc} &#36;|
|开方|\sqrt|$\sqrt {a+b}$|&#36; \sqrt {a+b} &#36;|
|开n次方|\sqrt[n]{m}|$\sqrt[3] {a+b}$|&#36; \sqrt[3] {a+b} &#36;|
|对数|\log|$\log(x)$|&#36; \log(x) &#36;|
|对数|\ln|$\ln(x)$|&#36; \ln(x) &#36;|以e为底|
|对数|\lg|$\lg(x)$|&#36; \lg(x) &#36;|以10为底|
|极限|\lim|$\lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$|&#36; \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}} &#36;|
|极限|\displaystyle \lim|$\displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}}$|&#36; \displaystyle \lim^{x \to \infty}_{y \to 0}{\frac{x}{y}} &#36;|
|求和|\sum|$\sum_{i=1}^n$|&#36; \sum_{i=1}^n &#36;|
|求和|\displaystyle \sum|$\displaystyle \sum_{i=1}^n$|&#36; \displaystyle \sum_{i=1}^n &#36;|
|累乘|\prod|$\prod_{i=1}^{n}$|&#36; \prod_{i=1}^{n} &#36;|
|余积|\coprod|$\coprod_{i=1}^{n}$|&#36; \coprod_{i=1}^{n} &#36;|
|最大|\max|$\max(a, b)$|&#36; \max(a, b) &#36;|
|最小|\min|$\min(a, b)$|&#36; \min(a, b) &#36;|
|上取整|\lceil 和 \rceil|$\lceil x \rceil$|&#36; \lceil x \rceil &#36;|
|下取整|\lfloor 和 \rfloor|$\lfloor x \rfloor$|&#36; \lfloor x \rfloor &#36;|

### 三角函数

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|度|\circ|$45^\circ$|&#36; 45^\circ &#36;|
|夹角|\angle|$\angle ACB$|&#36; \angle ACB &#36;|
|垂直|\bot|$L1 \bot L2$|&#36; L1 \bot L2 &#36;|
|sin|\sin|$\sin(45^\circ)={{\sqrt 2} \over 2}$|&#36; \sin(45^\circ)={{\sqrt 2} \over 2} &#36;|
|cos|\cos|$\cos(45^\circ)={{\sqrt 2} \over 2}$|&#36; \cos(45^\circ)={{\sqrt 2} \over 2} &#36;|
|tan|\tan|$\tan(45^\circ)={1 \over 2}$|&#36; \tan(45^\circ)={1 \over 2} &#36;|
|cot|\cot|$\cot(45^\circ)={1 \over 2}$|&#36; \cot(45^\circ)={1 \over 2} &#36;|
|sec|\sec|$\sec(45^\circ)={1 \over 2}$|&#36; \sec(45^\circ)={1 \over 2} &#36;|
|csc|\csc|$\csc(45^\circ)={1 \over 2}$|&#36; \csc(45^\circ)={1 \over 2} &#36;|

### 方程组

包含在 `\begin{cases}` 和 `\end{cases}` 之间，例如

$$
\begin{cases}
a_1x+b_1y+c_1z=d_1\\
a_2x+b_2y+c_2z=d_2\\
a_3x+b_3y+c_3z=d_3\\
\end{cases}
$$

``` markdown
$$
\begin{cases}
a_1x + b_1y + c_1z = d_1\\
a_2x + b_2y + c_2z = d_2\\
a_3x + b_3y + c_3z = d_3\\
\end{cases}
$$
```

### 分段函数

$$
P(x|Pa_x)=\begin{cases} 
1, & x=f(Pa_{x}) \\
0, & \text{other values}
\end{cases} \tag{9}
$$

```
$$
P(x|Pa_x)=\begin{cases} 
1, & x=f(Pa_{x}) \\
0, & \text{other values}
\end{cases} \tag{9}
$$
```

### 无穷大

|运算符|符号|示例|
|:-:|:-:|:-:|
|无穷大|\infty|$\infty$|
|正无穷|+\infty|$+\infty$|
|负无穷|-\infty|$-\infty$|

### 导数

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|一阶导数|\dot{a}|$\dot{a}$|&#36; \dot{a} &#36;|
|二阶导数|\ddot{a}|$\ddot{a}$|&#36; \ddot{a} &#36;|

### 微积分

- 微分

    |运算符|符号|示例|代码|
    |:-:|:-:|:-:|:-:|
    |微分|\partial|$\frac{\partial x}{\partial y}$|&#36; \frac{\partial x}{\partial y} &#36;|

- 积分

    |运算符|符号|示例|代码|
    |:-:|:-:|:-:|:-:|
    |积分|\int|$\int_{r=1}^\infty$|&#36; \int_{r=1}^\infty &#36;|
    |积分|\displaystyle \int|$\displaystyle \int_{r=1}^\infty$|&#36; \displaystyle \int_{r=1}^\infty &#36;|
    |双重积分|\iint|$\iint$|&#36; \iint &#36;|
    |三重积分|\iiint|$\iiint$|&#36; \iiint &#36;|

### 等号对齐

- 在 `\begin{aligned}` 和 `\end{aligned}` 之间
- 行末尾标记 `\\`
- 等号前加 `&` 符号

例如

$$
\begin{aligned} 
z_1 &= (a_1 + b_1i) \\ 
z_2 &= (a_2 + b_2i) \\
z_1z_2 &= (a_1 + b_1i)(a_2 + b_2i) \\
&= a_1a_2 + a_1b_2i + b_1a_2i + b_1b_2i^2 \\
&= (a_1a_2 - b_1b_2) + (a_1b_2 + b_1a_2)i 
\end{aligned}
$$

``` markdown
$$
\begin{aligned} 
z_1 &= (a_1 + b_1i) \\ 
z_2 &= (a_2 + b_2i) \\
z_1z_2 &= (a_1 + b_1i)(a_2 + b_2i) \\
&= a_1a_2 + a_1b_2i + b_1a_2i + b_1b_2i^2 \\
&= (a_1a_2 - b_1b_2) + (a_1b_2 + b_1a_2)i 
\end{aligned}
$$
```

### 其他符号

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|任取|\forall|$\forall$|&#36; \forall &#36;||
|存在|\exists|$\exists$|&#36; \exists &#36;||
|因为|\because|$\because$|&#36; \because &#36;||
|所以|\therefore|$\therefore$|&#36; \therefore &#36;||

## 向量

|运算符|符号|示例|代码|说明|
|:-:|:-:|:-:|:-:|:-:|
|向量|\vec|$\vec{a}$|&#36; \vec{a} &#36;||
|向量|\mathbf|$\mathbf{a}$|&#36; \mathbf{a} &#36;|粗体|

## 矩阵

- 在 `\begin{matrix}` 和 `\end{matrix}` 之间
- 行末尾标记 `\\`
- 行间元素用 `&` 分隔

### 常见形式

$$
\begin{matrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{matrix}
$$

``` markdown
$$
\begin{matrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{matrix}
$$
```

$$
\begin{pmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{pmatrix}
$$

``` markdown
$$
\begin{pmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{pmatrix}
$$
```

$$
\begin{bmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{bmatrix}
$$

``` markdown
$$
\begin{bmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{bmatrix}
$$
```

$$
\begin{Bmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{Bmatrix}
$$

``` markdown
$$
\begin{Bmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{Bmatrix}
$$
```
    
### 省略元素

- 横省略号：\cdots
- 竖省略号：\vdots
- 斜省略号：\ddots

例如

$$
\begin{bmatrix}
{a_{11}}&{a_{12}}&{\cdots}&{a_{1n}}\\
{a_{21}}&{a_{22}}&{\cdots}&{a_{2n}}\\
{\vdots}&{\vdots}&{\ddots}&{\vdots}\\
{a_{m1}}&{a_{m2}}&{\cdots}&{a_{mn}}\\
\end{bmatrix}
$$

```
$$
\begin{bmatrix}
{a_{11}}&{a_{12}}&{\cdots}&{a_{1n}}\\
{a_{21}}&{a_{22}}&{\cdots}&{a_{2n}}\\
{\vdots}&{\vdots}&{\ddots}&{\vdots}\\
{a_{m1}}&{a_{m2}}&{\cdots}&{a_{mn}}\\
\end{bmatrix}
$$
```

### 小矩阵

一般在行内公式中使用

这是一个小矩阵：$\left( \begin{smallmatrix} a & b \\ c & d \end{smallmatrix} \right)$

```
这是一个小矩阵：$\left( \begin{smallmatrix} a & b \\ c & d \end{smallmatrix} \right)$
```

> [!WARNING]
> github不支持小矩阵

### 增广矩阵

增广矩阵并不是按照标准的矩阵语法来实现的，先看个例子

$$ 
\left[
\begin{array}
{lcr|c}
a_{11} & a_{12} & a_{13} & b_1 \\
a_{21} & a_{22} & a_{23} & b_2 \\
a_{31} & a_{32} & a_{33} & b_3
\end{array}
\right]
$$

```
$$ 
\left[
\begin{array}
{lcr|c}
a_{11} & a_{12} & a_{13} & b_1 \\
a_{21} & a_{22} & a_{23} & b_2 \\
a_{31} & a_{32} & a_{33} & b_3
\end{array}
\right]
$$
```

**语法说明**
- 最外层 `\left` 及 `\right` 后的符号是阵列外符号，可以用(),[],|等
- `\begin` 及 `\end` 后用 `{array}` 声明阵列
- `{lcr|c}` 中每个字母代表一列（`l` 左对齐，`c` 居中，`r` 右对齐）；竖线 `|` 的位置会体现在矩阵中
- 元素之间同样用 `&` 分隔

> [!WARNING]
> github对增广矩阵的支持不完整，竖线没有渲染出来

### 行列式

$$
\begin{vmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{vmatrix}
$$

``` markdown
$$
\begin{vmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{vmatrix}
$$
```
### 矩阵范数

$$
\begin{Vmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{Vmatrix}
$$

``` markdown
$$
\begin{Vmatrix}
0&1&1\\
1&1&0\\
1&0&1\\
\end{Vmatrix}
$$
```

## 集合

### 符号

|名称|code|示例|代码|
|:-:|:-:|:-:|:-:|
|实数集| \mathbb{R} |$\mathbb{R}$|&#36; \mathbb{R} &#36;|
|复数集| \mathbb{C} |$\mathbb{C}$|&#36; \mathbb{C} &#36;|
|整数集| \mathbb{Z} |$\mathbb{Z}$|&#36; \mathbb{Z} &#36;|
|自然数集| \mathbb{N} |$\mathbb{N}$|&#36; \mathbb{N} &#36;|
|正整数集| \mathbb{W} |$\mathbb{W}$|&#36; \mathbb{W} &#36;|
|质数集| \mathbb{P} |$\mathbb{P}$|&#36; \mathbb{P} &#36;|
|有理数集| \mathbb{Q} |$\mathbb{Q}$|&#36; \mathbb{Q} &#36;|
|无理数集| \mathbb{I} |$\mathbb{I}$|&#36; \mathbb{I} &#36;|
|空集| \emptyset |$\emptyset$|&#36; \emptyset &#36;|

### 运算

|名称|code|示例|代码|
|:-:|:-:|:-:|:-:|
|属于|\in|$x \in y$|&#36; x \in y &#36;|
|不属于|\notin|$x \notin y$|&#36; x \notin y &#36;|
|包含于|\subset|$x \subset y$|&#36; x \subset y &#36;|
|包含|\supset|$x \supset y$|&#36; x \supset y &#36;|
|真包含于|\subseteq|$x \subseteq y$|&#36; x \subseteq y &#36;|
|真包含|\supseteq|$x \supseteq y$|&#36; x \supseteq y &#36;|
|交集|\cap|$A \cap B$|&#36; A \cap B &#36;|
|并集|\cup|$A \cup B$|&#36; A \cup B &#36;|
|差集|\setminus|$A \setminus B$|&#36; A \setminus B &#36;|

> [!NOTE]
> 差集也可以直接用 `-` 号，即 `$A-B$` 也表示差集 $A-B$

## 排列组合

|运算符|符号|示例|代码|
|:-:|:-:|:-:|:-:|
|排列|\binom {上位公式}{下位公式}|$\binom {n+1}{2k}$|&#36; \binom {n+1}{2k} &#36;|
|排列|{上位公式 \choose 下位公式}|${{n+1} \choose {2k}}$|&#36; {{n+1} \choose {2k}} &#36;|
|组合|{上位公式 \atop 下位公式}|$\sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots$|&#36; \sum_{k_0,k_1,\ldots>0 \atop k_0+k_1+\cdots=n}A_{k_0}A_{k_1}\cdots &#36;|