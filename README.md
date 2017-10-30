# A-few-days

A few days ?

Problem Description

给定一个日期，输出这个日期是该年的第几天。

 
Input

输入数据有多组，每组占一行，数据格式为YYYY/MM/DD组成，具体参见sample input ,另外，可以向你确保所有的输入数据是合法的。 


Output

对于每组输入数据，输出一行，表示该日期是该年的第几天。

 
Sample Input

1985/1/20

2006/3/12 


Sample Output

20

71 

解答：

#include<stdio.h>

main()

{

    int a,b,c,d,e,f,g;
    
    while(scanf("%d/%d/%d",&a,&b,&c)!=EOF)
    
    {
    

        if(b==1)
        
        d=c;
        
        else if(b==2)
        
        d=31+c;
        
        else if(b==3)
        
        d=31+28+c;
        
        else if(b==4)
        
        d=31+28+31+c;
        
        else if(b==5)
        
        d=31+31+28+30+c;
        
        else if(b==6)
        
        d=31+28+31+30+31+c;
        
        else if(b==7)
        
        d=31+28+31+30+31+30+c;
        
        else if(b==8)
        
        d=31+28+31+30+31+30+31+c;
        
        else if(b==9)
        
        d=31+28+31+30+31+30+31+31+c;
        
        else if(b==10)
        
        d=31+28+31+30+31+30+31+31+30+c;
        
        else if(b==11)
        
        d=31+28+31+30+31+30+31+31+30+31+c;
        
        else if(b==12)
        
        d=31+28+31+30+31+30+31+31+30+31+c+30;
        
          e=a%100;
          
        f=a%400;
        
        g=a%4;
        
        if(e==0)
        
        {
        
            if(f==0)
            
            d=1+d;
            
            else
            
            d=d;
            
        }
        
        else if(g=0)
        
        d=d+1;
        
        else
        
        d=d;
        
        printf("%d\n",d);
        

    }
    
}
