
#include <stdio.h>
int function(int n1,int n2)
{
    int gcd;
    for(int i=1;i<=n1&&i<=n2;i++)
    {
        if(n1%i==0&&n2%i==0)
        gcd=i;
    }
    return gcd;
}

int main()
{
    int t,n1,n2,result;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d",&n1,&n2);
        result=function(n1,n2);
        printf("%d",result);
    }
    

    return 0;
}
