#include<stdio.h>
int main()
{
    int n;
    
    int a[100];
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    int total=(n+1)*(n+2)/2;
    for(int j=0;j<n;j++)
    {
        total=total-a[j];
    }
    printf("%d",total);
}
