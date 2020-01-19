#include<stdio.h>
int main()
{
    int t,m,y,d;
    scanf("%d",&t);
    while(t--)
    {
      scanf("%d:%d:%d",y,m,d);
      if (m==4||m==6||m==9||m==11)
      {
          if (d%2==0)
          printf("%d",(61-d)/2);
          else if(d==30)
          printf("%d",2);
          else
          printf("%d",(61-d)/2+1);
      }
      else if(m==1||m==3||m==5||m==7||m==8||m==10||m==12)
      {
          if(d%2==0)
          printf("%d",(61-d)/2-1);
          //else if(d==31)
          printf("%d",1);
          else
          printf("%d",(61-d)/2);
          
      }
       else if(m==2) 
       {
           if(y%400==0||(y%100!=0&&y%4==0))
           printf("%d\n",(29-d)/2+1);
	        else
	        printf("%d\n",(59-d)/2+1);
       }
          
      
    }
    return 0;
}

