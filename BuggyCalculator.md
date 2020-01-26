#include<stdio.h>
int main()
{
int t,a,b,j,x,y,z,f,i;
scanf("%d\n",&t);
for(i=0;i<t;i++)
{
    f=0;
    j=1;
   scanf("%d",&a);
   scanf("%d",&b);
   while(a>0||b>0)
   {
       x=a%10;
       y=b%10;
       z=x+y;
       z=z%10;
       f=f+j*z;
       j=j*10;
       a=a/10;
       b=b/10;
   }
   printf("%d\n",f);
}
return 0;
}
