#include<stdio.h>
int function(int n)

{
    int three,two,four;
    two=n/2;
    three=n/3;
    four=n/4;
    int sum=0;
    sum=sum+three+four+two;
    return sum;
}
int main()
{
    int n,t;
    scanf("%d",&t);
    while(t--)
    {
    scanf("%d",&n);
    int sum;
    sum=function(n);
    if(sum<n)
    {
        printf("%d",n);
    }
    else {
        printf("%d",sum);
    }
    }
    
}
