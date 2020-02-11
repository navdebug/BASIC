#include<stdio.h>
int main()
{
    int t,n,k;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d",&n,&k);
        int a[n];
        for(int i=0;i<n;i++)   
        {
            scanf("%d",&a[i]);
        }
       int  min=a[0];
        for(int u=0;u<n;u++)
        {
            if(a[u]<=min)
            min=a[u];
        }
        if(k>=min)
        printf("%d",k-min);
        else
        printf("0\n");
    }
    return 0;
}
