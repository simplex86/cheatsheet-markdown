# 基础语法

- [标题](#标题)
- [目录](#目录)
    - [文档内跳转](#文档内跳转)
    - [跨文档跳转](#跨文档跳转)
    - [跨文档锚点](#跨文档锚点)
- [普通文本](#普通文本)
    - [文本颜色](#文本颜色)
    - [文本底色](#文本底色)
    - [文本对齐](#文本对齐)
- [字体](#字体)
- [段落与换行](#段落与换行)
- [引用](#引用)
- [警告](#警告)
- [列表](#列表)
    - [有序列表](#有序列表)
    - [无序列表](#无序列表)
    - [列表嵌套](#列表嵌套)
- [待办清单](#待办清单)
- [分隔线](#分隔线)
- [删除线](#删除线)
- [下划线](#下划线)
- [超链接](#超链接)
- [表格](#表格)
    - [表格对齐](#表格对齐)
- [图片](#图片)
    - [图片尺寸](#图片尺寸)
    - [图片对齐](#图片对齐)

## 标题

``` markdown
# 标题文本
```

- 在**行首**插入 `#` 可标记出标题
- `#` 的个数代表标题的等级，最多支持六级标题
- 在最后一个 `#` 后要加一个**空格**

## 目录

目录可在当前文档中跳转，也可以跳转到其他文档中

#### 文档内跳转

``` markdown
[目录文本](#标题文本)
```

[点击跳转到目录](#目录)

``` markdown
[点击跳转到目录](#目录)
```

> 注1：只能跳转到标题  
> 注2：不要漏掉了`#`号

#### 跨文档跳转

``` markdown
[目录文本](文档路径)
```

[点击跳转到公式编辑](../formula/formula.md)

``` markdown
[点击跳转到公式编辑](../formula/formula.md)
```

> [!NOTE]
> 文档路径可以是`绝对路径`，也可以是`相对路径`

#### 跨文档锚点

``` markdown
[目录文本](文件路径#锚点标题)
```

[点击跳转到公式编辑-矩阵](../formula/formula.md#矩阵)

``` markdown
[点击跳转到公式编辑-矩阵](../formula/formula.md#矩阵)
```

> 注1：仅支持跳转到markdown文件，因为需要识别标题

## 普通文本

``` markdown
普通文本
```
> [!NOTE]
> 不添加任何标记就是普通文本

#### 文本颜色

markdown 本身不支持`文本颜色`的语法，但`在支持HTML的环境中`可以使用`HTML标签`来实现

``` html
<font color=颜色>文本</font>
```

<font color=blue>蓝色的文本</font>

``` html
<font color=blue>蓝色的文本</font>
```

<font color=#ff0000>红色的文本</font>

``` html
<font color=#ff0000>红色的文本</font>
```

#### 文本底色

markdown 本身不支持`文本底色`的语法，但`在支持HTML的环境中`可以使用`HTML标签`来实现

``` html
<table><tr><td bgcolor=颜色>文本</td></tr></table>
```

<table><tr><td bgcolor=#007f00>绿油油的文本底色</td></tr></table>

``` html
<table><tr><td bgcolor=#00ff00>绿油油的文本底色</td></tr></table>
```

#### 文本对齐

markdown 本身不支持`文本对齐方式`的语法，但`在支持HTML的环境中`可以使用`HTML标签`来实现

- 左对齐

    <div style="text-align:left">左对齐文本</div>

    ``` html
    <div style="text-align:left">左对齐文本</div>
    ```

- 居中对齐

    <div style="text-align:center">居中对齐文本</div>

    ``` html
    <div style="text-align:center">居中对齐文本</div>
    ```

- 右对齐

    <div style="text-align:right">右对齐文本</div>

    ``` html
    <div style="text-align:right">右对齐文本</div>
    ```

## 字体

|字体|代码|
|----|---|
|*斜体*|\*斜体\*|
|**加粗** |\*\*加粗\*\* |
|***粗斜体***|\*\*\*粗斜体\*\*\* |

> [!NOTE]
> `*`与`*`之间、`*`与`文本`之间，不能有**空格**

## 段落与换行

段落由一行或多行文本组成，不同的段落之间使用空行来标记

- 如果行间**无空行**，则会被视为**同一段落**
- 如果行间**有空行**，则会被视为**不同段落**
- 如果想在**段内换行**，需要在行尾插入**两个（及以上的）空格**

## 引用

> 单行引用

``` markdown
> 单行引用
```

> 多行引用的第一行，我的最后有两个空格  
多行引用的结束行，后面没有空格了

``` markdown
> 多行引用的第一行，我的最后有两个空格  
多行引用的结束行，后面没有空格了
```

> 嵌套引用
>> 嵌套引用
>>> 嵌套引用

``` markdown
> 嵌套引用
>> 嵌套引用
>>> 嵌套引用
```

- 在引用中可以**嵌套**引用
- 在引用中可以使用其他的 markdown 语法
- 段落与换行的格式在引用中也是适用的

> [!NOTE]
> 嵌套引用建议不要超过三个层次

## 警告

警告的格式与引用类似，可分为5类

> [!NOTE]
> 用户应该知道的有用信息

``` markdown
> [!NOTE]
> 用户应该知道的有用信息
```

> [!TIP]
> 把事情做得更好或更容易的有用建议

``` markdown
> [!TIP]
> 把事情做得更好或更容易的有用建议
```

> [!IMPORTANT]
> 用户实现目标所需要知道的关键信息

``` markdown
> [!IMPORTANT]
> 用户实现目标所需要知道的关键信息
```

> [!WARNING]
> 需要用户立即注意以避免问题的紧急信息

``` markdown
> [!WARNING]
> 需要用户立即注意以避免问题的紧急信息
```

> [!caution]
> 就某些行为的风险或负面结果提供建议

``` markdown
> [!CAUTION]
> 就某些行为的风险或负面结果提供建议
```

需要说明的是，这几个关键字是大小写无关的！

## 列表

#### 有序列表

``` markdown
 数字序号. 列表内容
```
> [!NOTE]
> `.`和`文本`之间有个**空格**

1. 第一
2. 第二
3. 第三

``` markdown
1. 第一
2. 第二
3. 第三
```

#### 无序列表

``` markdown
- 列表内容
```

> [!TIP]
> `-`和`文本`之间有个**空格**

- 第一
- 第二
- 第三

``` markdown
- 第一
- 第二
- 第三
```

#### 列表嵌套

- 缩进使用`Tab`键
- 有序列表和无序列表也可互相嵌套

> [!WARNING]
> 建议最多嵌套三层

- 第一层列表
    - 第二层列表
        - 第三层列表

``` markdown
- 第一层列表
    - 第二层列表
        - 第三层列表
```

## 待办清单

``` markdown
- [ ] 未勾选
- [x] 已勾选
```

- 当中括号中的字符为**空格**时，复选框是`未选中`状态
- 当中括号中的字符为 `x` 时，复选框是`已选中`状态

> [!NOTE]
> `x`使用小写

今日计划：
- [x] 吃
    - [x] 吃瓜
    - [ ] 吃鸡
- [x] 喝
- [ ] 玩
- [ ] 乐

``` markdown
今日计划：
- [x] 吃
    - [x] 吃瓜
    - [ ] 吃鸡
- [x] 喝
- [ ] 玩
- [ ] 乐
```

> [!NOTE]
> 待办清单是可以嵌套的

## 分隔线

``` markdown
---
```

> [!NOTE]
> 分隔线须使用`至少3个`以上的`-`来标记

## 删除线

``` markdown
~~被删除的内容~~
```

> [!NOTE]
> `~`和`~`之间、`~~`和`文本`之间没有**空格** 

她每天都要刷一小时短视频，~~做10道题~~

``` markdown
她每天都要刷一小时短视频，~~做10道题~~
```

## 下划线

``` html
<u>下划线</u>
```

> [!WARNING]
> 非 markdown 原生语法，不是所用markdown引擎都支持

注意<u>划重点</u>，都是考点

``` markdown
注意<u>划重点</u>，都是考点
```

## 超链接

``` markdown
[链接文字](链接地址)
```

常用网站：[知乎](https://www.zhihu.com/)、[B站](https://www.bilibili.com/)

``` markdown
常用网站：[知乎](https://www.zhihu.com/)、[B站](https://www.bilibili.com/)
```

## 表格

``` markdown
|表头1|表头2|表头3|
|-----|-----|-----|
|内容1|内容2|内容3|
|内容1|内容2|内容3|
|内容1|内容2|内容3|
```

- 在每一行最前和最后都使用`|`，每一行中的 `|` 要尽量都对齐
- 表头与其他行使用（多个）`-` 来分隔

|序号|网站|网址|
|----|----|----|
|01|知乎|https://www.zhihu.com|
|02|B站|https://www.bilibili.com|

``` markdown
|序号|网站|网址|
|----|----|----|
|01|知乎|https://www.zhihu.com|
|02|B站|https://www.bilibili.com|
```

#### 表格对齐

- `:-` 左对齐（默认） 
- `-:` 右对齐 
- `:-:` 居中对齐 

|左对齐|居中对齐|右对齐|
|:----|:----:|----:|
|01|知乎|https://www.zhihu.com|
|02|B站|https://www.bilibili.com|

``` markdown
|左对齐|居中对齐|右对齐|
|:----|:----:|----:|
|01|知乎|https://www.zhihu.com|
|02|B站|https://www.bilibili.com|
```

> [!NOTE]
> A. 块级元素（代码区块、引用区块）不能插入表格中  
> B. 不要使用庞大复杂的表格，那样会难以维护和阅读

## 图片

``` markdown
![图片替换文字](图片地址)
```

- 图片替代文字在图片`无法正常显示`时会比较有用，一般情况下可为空
- 图片地址可以是`本地图片路径`也可以是`网络图片路径`
- 本地图片支持`相对路径`和`绝对路径`两种方式

![本地图片_相对路径](./imgs/image_01.jpeg)

``` markdown
![本地图片_相对路径](./imgs/image_01.jpeg)
```

> [!TIP]
> 不要漏掉开头的 `!` 号

#### 图片尺寸

markdown 本身不支持`图片尺寸`的语法，但`在支持HTML的环境中`可以使用`HTML标签`来实现

- 绝对尺寸

    <img src="./imgs/image_01.jpeg" width=100 height=100 />

    ``` html
    <img src="./imgs/image_01.jpeg" width=150 height=150 />
    ```

- 相对尺寸

    <img src="./imgs/image_01.jpeg" width=20% height=20% />

    ``` html
    <img src="./imgs/image_01.jpeg" width=20% height=20% />
    ```

#### 图片对齐

markdown 本身不支持`对齐方式`的语法，但`在支持HTML的环境中`可以使用`HTML标签`来实现

- 左对齐

    <div align="left"> <img src="./imgs/image_01.jpeg" width=20% height=20% /> </div>

    ``` html
    <div align="left"> <img src="./imgs/image_01.jpeg" width=20% height=20% /> </div>
    ```

> [!NOTE]
> 左对齐是 markdown 默认的对齐方式

- 居中对齐

    <div align="center"> <img src="./imgs/image_01.jpeg" width=20% height=20% /> </div>

    ``` html
    <div align="center"> <img src="./imgs/image_01.jpeg" width=20% height=20% /> </div>
    ```

- 右对齐

    <div align="right"> <img src="./imgs/image_01.jpeg" width=20% height=20% /> </div>

    ``` html
    <div align="right"> <img src="./imgs/image_01.jpeg" width=20% height=20% /> </div>
    ```