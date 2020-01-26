#include<stdio.h>
void function()
{
    int t,n,ans=0,a,b;
    while(t--)
    {
        scanf("%d",&n);
        for(int i=0;i<n;i++)
        {
            scanf("%d%d",&a,&b);
           ans=ans^i; 
        }
    }
}
int main()
{
    function();
    return 0;
}
