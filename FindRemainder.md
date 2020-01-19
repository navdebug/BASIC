#include<stdio.h>
int main()
{
    int t,r,n;
    scanf("%d",&t);
    for(int i=1;i<=t;i++)
    {
     scanf("%d%d",&n,&r);
     printf("%d",n%r);
     
    }
    return 0;
}
