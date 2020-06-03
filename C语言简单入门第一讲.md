# *C语言简单入门**

首先下载一个编程软件例如Dev-C++或者VS等等

下载网址为链接：https://pan.baidu.com/s/1W9-O46dJZZTwJ2cwHaoq2g 
             提取码：642b

入门第一堂课hello world

#include<stdio.h>是C语言编译的预处理指令

 int main() 

{

}

int main为主函数，运行主要程序，程序一般放入大括号中，

**C语言程序必须包含唯一一个main函数且程序执行必须由main函数开始，到main函数结束**

在C语言中每行程序写完需要加上一个分号（英文输入法输入的）以示结束，

printf是c语言的一个关键词，意思是打印，

将你要打印的代码写入括号里并标上双引号，例如printf（“hello world”）；意思是会在编辑后的命令窗口打印出hello world

return 0 是返回值语句，它会在主函数结尾写入

双斜杠//的意义是注释，你可以将中英文写在//的后面，他将不会影响程序的运行/*     */ 是多行注释

hello world的实例程序

#include<stdio.h>

 int main() 
{        
       printf（"hello world"）;//打印hello world
       
       return 0;
}

当你运行程序就会出现以下内容

![2020-05-04](C:\Users\23937\Desktop\2020-05-04.png)

Dec-c++软件初步使用方法![Inked2020-05-04 (1)_LI](C:\Users\23937\Desktop\Inked2020-05-04 (1)_LI.jpg)

在程序写完后点击图片左侧画圈的编译按钮，检查错误

之后点击右侧画圈的编译运行按钮，检查错误并弹出命令窗口如第一个图。
