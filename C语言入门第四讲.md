# C语言入门第四讲

##### 逻辑量的真假判定──０和非０

Ｃ语言用整数"１"表示"逻辑真"、用"０"表示"逻辑假"。但在判断一个数据的"真"或"假"时，却以０和非０为根据：  

如果为０，则判定为"逻辑假"；如果为非０，则判定为"逻辑真"。  

例如，假设num=12，则： ！num的值=０ ，num>=1 ＆＆ num<=31的值=１ ，num || num>31的值=1。  

逻辑运算的值也为“真”和“假”两种，用“1”和“0 ”来表示。其求值规则如下：  

（1）与运算 &&：参与运算的两个量都为真时，结果才为真，否则为假。  

（2）或运算||：参与运算的两个量只要有一个为真，结果就为真。两个量都为假时，结果为假。  

（3）非运算!：参与运算量为真时，结果为假；参与运算量为假时，结果为真。 虽然Ｃ编译在给出逻辑运算值时，以“1”代表“真”，“0 ”代表“假”。但反过来在判断一个量是为“真”还是为“假”时，以“0”代表“假”，以非“0”的数值作为“真”。

##### if语句

if是根据条件进行控制哪条语句的进行

结构 if（条件表达式）

​        {

​           复合语句A；

​        }

当if为一条简单语句时，可以省略{}即：

if（条件表达式）

​    简单语句A；

eg：

#include<stdio.h>

int main()

{

​	int age,price=80;

​	printf("请输入你的年龄：")；

​        scanf(“%d”，&age);

​        if(age>=60||age<=10)//年龄大于等于60和年龄小于等于6岁的执行下面的程序票价除以2

​        price/=2;

​        printf("你的年龄：%d，票价%d\n",age,price);

​	return 0;

}

##### if-else

if（条件表达式）

{

  复合语句A；

}

else

{

复合语句B；

}

在if的条件中判断，结果是真执行 复合语句A，结果是假，执行复合语句B；

#include <stdio.h>  

int main()  

{  

int age;  

printf(“请输入你的年龄：”);  

scanf("%d", &age);  

if(age>=18){  

printf(“恭喜，你已经成年，可以使用该软件！\n”);  

}else{  

printf(“抱歉，你还未成年，不宜使用该软件！\n”);  

}  

return 0;  

}  

可能的运行结果：

请输入你的年龄：23↙
恭喜，你已经成年，可以使用该软件！
1
2
或者：

请输入你的年龄：16
抱歉，你还未成年，不宜使用该软件！

##### if-else语句的嵌套

#include <stdio.h>

int main ( ) 
{ 

 double fuel_reading;  


    printf("输入油量表读数(0-1): ");  
    scanf("%lf", &fuel_reading); 
    
    //下面加上花括号使if-else能够正确匹配  
    if (fuel_reading < 0.75)  
    {  
        if (fuel_reading < 0.25)  
            printf("油量低，注意!\n");  
    }  
    else  
    {  
        printf("高油量，不必停!\n");  
    }  
    return 0;  
}  
}

