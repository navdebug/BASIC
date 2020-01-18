#include<stdio.h>
int main()
{
    int n,temp;
    scanf("%d",&n);
    temp=n;
    int dig=0;
    while(temp>0)
    {
        temp=temp/10;
        dig++;
    }
    printf("The number of digits in the given number is %d",dig);
    return 0;
}
