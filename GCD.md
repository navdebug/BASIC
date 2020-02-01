#include<stdio.h>
void function()
{
    int n1,n2;
    int gcd;
    scanf("%d%d",&n1,&n2);
    for(int i=1;i<=n1&&i<=n2;i++)
    {
        if(n1%i==0&&n2%i==0)
        gcd=i;
    }
    printf("%d",gcd);
}
int main()


{
    function();
    return 0;
}
