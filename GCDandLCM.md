#include<stdio.h>
int gcd(int n1,int n2)

{
    int g;
    for(int i=1;i<=n1&&i<=n2;i++)
    {
        if(n1%i==0&&n2%i==0)
        g=i;
    }
    return g;
}
int lcm(int n1,int n2)
{
    int min=(n1>n2)?n2:n1;
    while(1)
    {
        if(min%n1==0&&min%n2==0)
        {
        break;}
    
    min++;
    }
    return min;
}
int main()
{
    int t,g,l,n1,n2;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d",&n1,&n2);
       g=gcd(n1,n2);
       l=lcm(n1,n2);
       printf("%d\t%d",g,l);
    }
}
