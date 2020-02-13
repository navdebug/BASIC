
#include <stdio.h>
#include<math.h>
int gcd(int a,int b,int n)
{
    int g;
    int c= pow(a,n)+(b,n);
    int d=a-b;
    for(int i=1;i<=c&&i<=d;i++)
    {
        if(c%i==0&&d%i==0)
        g=i;
    }
    return g;
}
int main()
{
    int t;
    scanf("%d",&t);
    while(t--)
    {
        int a,b,n;
        scanf("%d%d%d",&a,&b,&n);
        int r=gcd(a,b,n);
        printf("%d",r);
    }

    return 0;
}
