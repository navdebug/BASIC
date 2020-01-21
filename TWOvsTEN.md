#include<stdio.h>
void function()
{
    int t,n,r=0;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d",&n);
        if(n%10==0)
        printf("0\n");
       else if(n%5==0)
         printf("1\n");
         else
         printf("-1\n");
    }
}
int main()
{
    function();
    return 0;
}
