#include<stdio.h>
#include<math.h>
void function()
{
    int t,n,z;
    scanf("%d",&t);
    while(t--)
    {
       scanf("%d",&n);
       z=sqrt(n);
       printf("%d",z);
       //printf("%d",sqrt(n));
    }
}
int main()
{
    function();
    return 0;
}
