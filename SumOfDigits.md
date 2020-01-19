#include<stdio.h>
int main()
{
    int t,temp,r,n,sum=0;
    scanf("%d",&t);
    for(int i=0;i<t;i++)
    {
        scanf("%d",&n);
        temp=n;
        while(temp!=0)
        {
            r=temp%10;
            
            sum=sum+r;
            temp=temp/10;
        }
        printf("The sum is %d",sum);
    }
    return 0;
}
