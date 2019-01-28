# Markdown编辑

Markdown | 语法 | 效果
--|--|--
Bold | `**text**` | **text**
Emphasize | `*text*` | *text*
Strike-through | `~~text~~` | ~~text~~
内嵌代码 | ``code`` | `code`
List | `* item` | * item
Blockquote | `> quote` | > quote
H1 | `# Heading` | # Heading
H2 | `## Heading` | ## Heading
H3 | `### Heading` | ### Heading
画水平线 | `--------` | --------
Link | `[github](https://github.com/)` | [github](https://github.com/)
Image | `![pic](http://)` | ![pic](http://)
标注 | `标注[^1]: This is my first footnote` | 标注[^1]: This is my first footnote

表格：

header 1 | header 2
---|---
row 1 col 1 | row 1 col 2
row 2 col 1 | row 2 col 2

## 公式编辑
- 空格  

Markdown | 语法 | 效果  
--|--|--  
两个quad空格 | a \qquad b | 两个m的宽度  
quad空格 | a \quad b | 一个m的宽度  
大空格 | a\\ b | 1/3m宽度  
中等空格 | a\;b | 2/7m宽度  
小空格 | a\,b | 1/6m宽度  
没有空格 | ab |  
紧贴 | a\\!b | 缩进1/6m宽度    


- 角标 和 开方
```
x=\frac{-b\pm\sqrt{b^2-4a_1c_1}}{2a}
```
$$
    x=\frac{-b\pm\sqrt[3]{b^2-4a_1c_1}}{2a}
$$

3. 求和与联乘
```
    \sum_{i=0}^{n}
    \sum^{n}_{j=0}
    \prod_{10}
    \prod_\epsilon
```
$$
    \sum_{i=0}^{n}
    \sum^{n}_{j=0}
    \prod_{10}
    \prod_\epsilon
$$

4. 微分与积分
```
    \int_{a}^{\pi}f(x)dx
```
$$
    \int_{a}^{\pi}f(x)dx
$$

5. 极限 与 偏导数
```
    \lim_{x \to +\infty}\frac{1}{x}
    \frac{\partial^2 u}{\partial z^2}
```
$$
    \lim_{x \to +\infty}\frac{1}{x}
    \frac{\partial^2 u}{\partial z^2}
$$

6. 三角函数与矩阵
```

    \cos2\theta = cos^2\theta - \sin^2 \theta \\ =  2\cos^2\theta -1

    \begin{equation}
    A=\left[
        \begin{matrix}
        1&2&3&\\
        2&2&3&\\
        3&2&3&
        \end{matrix}
    \right]
    \end{equation}
```
$$
    \cos2\theta = cos^2\theta - \sin^2 \theta = 2\cos^2\theta -1
    \begin{equation}
    A=\left[
        \begin{matrix}
        1&2&3&\\
        2&2&3&\\
        3&2&3&
        \end{matrix}
    \right]
    \end{equation}
$$

7. 分数
```
\frac{a-1}{b-1} 
或者
{a+1\over b+1}
```
$$
    \frac{a-1}{b-1} \quad and \quad {a+1\over b+1}
$$

[在线公式编辑页](https://www.codecogs.com/latex/eqneditor.php?lang=zh-cn)
[KATEX公式文档](https://katex.org/docs/supported.html)

![公式对照表1](/image/latex_1.png)
![公式对照表2](/image/latex_2.png)
![公式对照表3](/image/latex_3.png)












