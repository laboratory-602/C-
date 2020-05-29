### C语言入门第5讲

#### 选择语句switch ——case

switch(条件表达式)

{case常量表达式1:语句1;break;

 case常量表达式2:语句2;break;

 ...

case常量表达式n:语句n;break;

default:语句n+1;break;

}

eg:

#include<stdio.h>

int main(void)

{ int a=2,b=0;

 switch(a)

{   case 1:b++;

​    case 2:a=3;

​    case 3:b--;

​    default:a=4

}

printf("a=%d\n",a);

return 0;

}

输出a=3

#### 循环语句

##### while循环

while（判断条件）

{ 

循环体语句

}

eg:

#include<stido.h> 

int main()

{ 	int sum=0,i=1;

  	while(i<=100)

​        {

​		sum+=i;

​		i+=2;

}

printf("sum=%d\n",sum);

return 0;

}

结果sum=2500