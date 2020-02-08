#include<stdio.h>
void function()
{
    int n,max=0,x;
    scanf("%d",&n);
    int a[100];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(int i=0;i<n;i++)
    {
        for(int j=i-1;j>=0;j--)
        {
           x=a[i] &a[j];
           if(x>max)
           max=x;
        }
    }
    printf("%d",max);
}
int main()
{
    function();
    return 0;
}
