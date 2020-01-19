#include<stdio.h>
int main()
{
    int t,temp,n,r,rev=0,;
    scanf("%d",&t);
    
    for(int i=0;i<t;i++)
    {
        scanf("%d",&n);
        while(n!=0)
        {
            r=n%10;
            rev=rev*10+r;
            n=n/10;
            //printf("%d",rev);
        }
       
    }
    printf("%d\n",rev);
}
