#include<stdio.h>
int main()
{
    int t,temp,r,n,fact=1;
    scanf("%d",&t);
    for(int i=1;i<=t;i++)
    {
     scanf("%d",&n);
     for(int j=1;j<=n;j++)
     {
         fact=fact*j;
         
     }
     printf("%d",fact);
     
    }
    return 0;
}
