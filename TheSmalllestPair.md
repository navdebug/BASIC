#include<stdio.h>
void function()
{
    int t,n;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d",&n);
        int a[n];
        for(int i=0;i<n;i++)
        {
            scanf("%d",&a[i]);
        }
        int min=0;
        for(int i=0;i<n;i++)
        {
            if(a[i]<a[min])
            min=i;
        }
        int sum=0;
        sum=sum+a[min];
        printf("%d is the sum",sum);
        
    }
}
int main()
{
    function();
    return 0;
}
