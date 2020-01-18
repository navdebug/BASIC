#include<stdio.h>
int main()
{
    int n,r,temp;
    scanf("%d",&n);
    temp=n;

    while(temp>0)
    {
        r=temp%10;
        temp=temp/10;
        printf("Spilt numbers are %d\n",r);
    }
    
    return 0;
}
