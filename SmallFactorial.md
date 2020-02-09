#include<stdio.h>
int function(int n)
{
    int fact=1;
    
    for(int i=1;i<=n;i++)
    {
        fact=fact*i;
    }
    return fact;
}
int main()
{
    int t,n,result;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d",&n);
        result=function(n);
        printf("%d",result);
    }
}
