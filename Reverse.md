#include<stdio.h>
main()
{
    int n,r,rev=0;
    printf("Enter a number to reverse");
    scanf("%d",&n);
    while(n!=0)
    {
        r=n%10;
    
    rev=rev*10+r;
    n=n/10;
    }
    printf("the reversed number is %d",rev);
}
