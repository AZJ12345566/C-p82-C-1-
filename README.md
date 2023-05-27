# C-p82-C-1-
C语言学习笔记 p82 初始C语言（1）
主要编译器有：Clang（LLVM，Xcode的编译器）,GCC,WIN-TC,SUBLINE,MSVC,Turbo C等。
#include<stdio.h>
int main()//程序的入口
{
    char ch='A';//char为字符类型，字符用单引号
    //字符用%c来打印
    return 0;
}

bit,byte(8个bit),kb(1024个byte),mb(1024个kb),gb(1024mb),tb(1024gb),pb(1024tb)

int main()
{
    short age=20;//向内存申请2个字节存放age
    float weight=96.5f;//向内存申请4个字节来存放小数
    return 0;
}

int num2=20;//全局变量-定义在代码块（{}）之外的变量
int main()
{
    int num1;//局部变量-定义在代码块之内的变量
    return 0;
}
//全局变量和局部变量名字相同时，局部变量优先使用，所以建议全局变量不要和局部变量名字相同


int main()
{
    int num1=0;
    int num2=0;
    int sum=0;
    //输入数据-使用输入函数scanf
    scanf("%d%d",&num1,&num2);
    //C语言规定，变量要放在代码块最前面使用
    sum=num1+num2;
    printf("%d\n",sum);
    return 0;
}


变量的作业域和生命周期
1.局部变量的作用域是变量所在的局部范围
2.全局变量的作用域是整个工程，在头文件的全局变量可以在原文件声明之后使用


生命周期
1.局部变量的生命周期是：进入作用域生命周期开始，出作业域生命周期结束。
2.全局变量的生命周期是：整个程序的生命周期




Unix系统知识
Unix的主要特点是：高内聚，低耦合
Unix的命令行虽然复杂，但是命令相互支持，命令通过管道或重定向相互连接在一起
Unix比windows切换用户更加方便

