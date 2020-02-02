#include<stdio.h>
void function()
{
    int a[100],n,pos;
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    scanf("%d",&a[i]);
    scanf("%d",&pos);
    for(int i=pos-1;i<n-1;i++)
    {
    a[i]=a[i+1];
    }
    n--;
    for(int c=0;c<n;c++)
    printf("%d",a[c]);
    
}
int main()
{
    function();
    return 0;
}
