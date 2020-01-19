#include<stdio.h>
int main()
{
    int t,n,r,a,s[100];
    scanf("%d",&t);
    
    for(int i=0;i<t;i++)
    {
        scanf("%d",&n);
        r=n%10;
        while(n/10)
        {
            a=n/10;
            n=n/10;
        }
        s[i]=a+r;
        printf("%d\n",s[i]);
    }
    
    return 0;
}
