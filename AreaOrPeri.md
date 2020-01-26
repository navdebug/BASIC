#include<stdio.h>
void function()
{
    int l,b;
    scanf("%d",&l);
    scanf("%d",&b);
    int area=l*b;
    int peri = 2*(l+b);
    if (area>peri)
    {
    printf("area");
    printf("%d",area);
    }
    else
    {
    printf("peri\n");
    printf("%d",peri);
    }
}
int main()
{
    function();
    return 0;
}
