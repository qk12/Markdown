C语言
    ——从入门到放弃

[TOC]

**从一段程序开始**
```c
#include <stdio.h> //head
 
int main()
{
    // 我的第一个 C 程序
    printf("Hello, World!\n");

    return 0;
}
```

**程序解释**
* `stdio.h` 是一个头文件 (标准输入输出头文件) , `#include` 是一个预处理命令，用来引入头文件。 当编译器遇到 `printf()` 函数时，如果没有找到 `stdio.h` 头文件，会发生编译错误
* 所有的 C 语言程序都有且仅有一个 `main()` 函数。 代码从 `main()` 函数开始执行
* `//` 用于注释说明
* `printf()` 用于格式化输出到屏幕。`printf()` 函数在 `stdio.h` 头文件中声明
* `return 0;` 终止 `main()` 函数，并返回值 0

**C 程序主要包括以下部分**
* 预处理器指令
* 函数
* 变量
* 语句 & 表达式
* 注释


# C 数据类型


# C 变量
变量其实只不过是程序可操作的存储区的名称。C 中每个变量都有特定的类型，类型决定了变量存储的大小和布局，该范围内的值都可以存储在内存中，运算符可应用于变量上。

变量的名称可以由字母、数字和下划线字符组成。它必须以字母或下划线开头。大写字母和小写字母是不同的，因为 C 是大小写敏感的。基于前一章讲解的基本类型，有以下几种基本的变量类型：

char类型用于储存字符（如，字母或标点符号），但是从技术层面上看，char是整数类型，因为char类型实际上存储的是整数而不是字符。计算机使用数字编码来处理字符，即用特定的整数表示特定的字符。



# C 运算符
* 算术运算符
* 关系运算符
* 逻辑运算符
* 位运算符
* 赋值运算符





# C 判断
**if语句**
```cpp
if(/* 条件为true */)  
{
   // 执行
}
else if()
{
    // 执行
}
else () // 和 else if() 的区别？
{
    // 执行
}
```
**嵌套**
```c
if (a == 100)
   {
       if(b == 200)
       {
          // 执行
       }
   }
// 等价于
if (a == 100 && b == 200)
{

}
```
**swith语句**
```c
switch(expression)
{
    case constant-expression  :
       statement(s);
       break; /* 可选的 */
    case constant-expression  :
       statement(s);
       break; /* 可选的 */
  
    /* 您可以有任意数量的 case 语句 */
    default : /* 可选的 */
       statement(s);
}
```

# C 循环
循环控制语句
一般情况下，语句是按顺序执行的：函数中的第一个语句先执行，接着是第二个语句，依此类推。
```
while(condition)
{
   statement(s);
}
```

# C 函数
```c
#include <stdio.h>

int add(int a, int b);

int main()
{
    int a, b;
    scanf("%d%d",&a,&b);
    int c = add(a, b);
    printf("%d", c);
    return 0;
}

int add(int a, int b)
{
    int c = a + b;
    return c;
}
```

# C 字符串
在 C 语言中，字符串实际上是使用 null 字符 '\0' 终止的一维字符数组。因此，一个以 null 结尾的字符串，包含了组成字符串的字符。

下面的声明和初始化创建了一个 "Hello" 字符串。由于在数组的末尾存储了空字符，所以字符数组的大小比单词 "Hello" 的字符数多一个。

# C 文件读写
```c
FILE *fopen( const char * filename, const char * mode );
```

**使用C语言的7个步骤**
1. 定义程序的目标
2. 设计程序
3. 编写代码
4. 编译
5. 运行程序
6. 测试和调试程序
7. 维护和修改代码

