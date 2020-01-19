#include<stdio.h>
int main()
{
    int x;
    float y;
    //x is the amount of $US one wants to withdraw
    //y is bank balance
    scanf("%d %f",&x,&y);
    if((x%5==0)&&(x<y))
    {
        printf("%f",(y-x)-0.5);
    }
    else 
    {
        printf("Invalid withdrawal");
    }
    return 0;
}
