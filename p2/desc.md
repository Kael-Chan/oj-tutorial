<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>

## Problem 2

在上一题中，你提交了一份：
- 没有输入
- 会输出`Hello World!`

的程序，并拿到了100分。

online judge做的事情很简单：
- 给你的程序**特定的输入**，在此例中，输入为空
- 检查你的程序的**输出是否与预计的相同**
- 根据**每一组输入输出的正确性**，给出判断结果

下面尝试一道简单的题目：
- 输入：两个整数
- 输出：反序的两个整数

例：
- 输入：188 23
- 输出：23 188

**（醒目）助教不小心放在这里的错误答案 **

    #include<iostream>
    using namespace std;
    int main()
    {
        int a,b;
        cout<<"请输入两个整数：";
        cin>>a>>b;
        cout<<b<<a;
        return 0;
    }

提交以上代码文件，然后……你得到了0分！

假设输入为`188 23`，请体会以上代码的输出：
- 输入：188 23
- 输出：请输入两个整数：23188

由于输出与预计的不同，online judge视为错误。这看起来很死板，但不同人有不同的输入提示，没法一一考虑，应该选择一个**最简洁的方案**。

此外，23和188两个数字没有使用空白符（例如空格）隔开，显然不对（即使自己用肉眼看，也会把它当做一个五位数吧～）。

**（醒目）助教不小心放在这里的正确答案 **

    #include<iostream>
    using namespace std;
    int main()
    {
        int a,b;
        cin>>a>>b;
        cout<<b<<' '<<a;
        return 0;
    }

再次提交，就可以看到绿色的100分啦。

**对同一个题目，你可以多次提交，并在`All Submission`选项卡中为每道题选择一个`Final Submission`作为最终结果**
