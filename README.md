# C-language-
C language starting 
//first code
#include<stdio.h>
void main()
{
printf("hello world");
}
\\output
hello world 





#include<stdio.h>
void main()
{
    int a,b,sum,sub,mul,di;
    printf("enter number a and b");
    scanf(" %d%d",&a,&b);
    sum=a+b;
    printf("%d+%d=%d\n",a,b,sum);
    sub=a-b;
    printf("%d-%d=%d\n",a,b,sub);
    mul=a*b;
    printf("%d*%d=%d\n",a,b,mul);
    di=a/b;
    printf("%d+%d=%d\n",a,b,di)
}
\\output
enter number a and b
200
25
200+25=225
200-25-175
200*25=5000
200/25=8



//valid declaration 
int a,b,c;
a=b=c=5;
printf("%d\n%d\n%d\n",a,b,c);

#include <stdio.h>
void main()
{    
int a,b=2,c=3;
printf("%d\n",c%b);
printf("%d\n",-c%b);
}

//output
1
-1


