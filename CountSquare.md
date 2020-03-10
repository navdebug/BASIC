# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main()
{
    int t,square=1,c=0;
    scanf("%d",&t);
    while(t--)
    {
        int n;
        scanf("%d",&n);
        for(int i=1;i<n;i++)
        {
           square=i*i;
           if(square<n)
           c++;
        }
        printf("%d",c);
    }
}
