#include<stdio.h>
int main()
{
int t,n,r;
scanf("%d",&t);
for(int i=0;i<t;i++)
{
scanf("%d%d",&n,&r);
if(n<r)
printf("<");
else if(n>r)
printf(">");
else
printf("=");
}
return 0;
}
