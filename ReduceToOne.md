#include<stdio.h>
void function()
{
    int t;
    scanf("%d",&t);
    while(t--)
    {
        int n;
        scanf("%d",&n);
        int ans=n;
        for(int i=0;i<n;i++)
        {
            ans=i+ans*i+ans;
        }
        printf("%d",ans);
    }
}
int main()
{
    function();
    return 0;
}
