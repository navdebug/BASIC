# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main()
{
    int t;
    scanf("%d",&t);
    while(t--)
    {
        int n,d;
        scanf("%d%d",&n,&d);
        int a[n];
        for(int i=0;i<n;i++)
        scanf("%d",&a[i]);
        while(d--)   
        {
            int temp=a[0],j;
            for( j=0;j<n-1;j++)
            a[j]=a[j+1];
            a[j]=temp;
        }
        for(int h=0;h<n;h++)
        printf("%d\t",a[h]);
    }
    return 0;
}
