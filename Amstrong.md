#include<stdio.h>
main()
{
    int n,c,r,sum=0;
    printf("Enter an amstrong number");
    scanf("%d",&n);
    int temp=n;
    while(n!=0)
    {
        r=n%10;
        c=r*r*r;
        sum=sum+c;
        n=n/10;
    }
    if(sum==temp)
    printf("Entered number is an amstrong number");
}
