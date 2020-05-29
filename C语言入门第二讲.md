# C语言学习第二讲

### ANIS C标准提供了32个关键字

int char float double void short long signed unsigned struct union enum typedef sizeof auto static

register extern const  volatile continue return break goto if else switch case default for do while

### 常量和变量

常量：数值变量：1 ，2 .1等

​           字符变量：使用单引号括起来一个符号如‘a'、’#‘等

​           字符串变量：双引号括起来若干字符”hello world“

​            符号变量：使用宏定义符号常量，如 #define PI 3.1415926

变量：可以改变的量

变量的定义形式为 类型名 变量名【=初始值】

eg:  int a=3;//定义了整型变量a并使a=3

类型名 int 整型       float单精度浮点型     double 双精度浮点型（浮点型就是定义小数时使用double比float的位数多）

转义字符有十三个

最为常用的试 \n 换行会把之后写的程序转到下一行

### 格式输入输出

％d整型输出，％ld长整型输出，

％o以八进制数形式输出整数，

％x以十六进制数形式输出整数，

％u以十进制数输出unsigned型数据(无符号数)。

％c用来输出一个字符

％s用来输出一个字符串，

％f用来输出实数，以小数形式输出

％e以指数形式输出实数，

printf（”格式符“，输出地址）eg：printf（”%d“，a）；

输入 scanf （”格式符“，输入地址）eg：scanf （”%d“，a）；

C语言的运算顺序是从右到左

##### 代码

#include<stdio.h>

int main()

{     int a=3，b=5；

​      printf("a=%d,b=%d",a,b);

​      return 0;

}

输出结果a=3，b=5

#include<stdio.h>

int main()

{     int a;

​      scanf（”%d“,&a）;

​      printf("a=%d",a);

​      return 0;

}

输入3

输出结果a=3

#include<stdio.h>

int main()

{     char a='b';

​      printf("%c,%d",a,a);

​      return 0;

}

输出b，98 因为变量a存储为01100010



