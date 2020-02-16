
#include <stdio.h>
int function(int n,int m)
{
    int c=0;
    for(int i=n;i<m;i++)
    if(i%10==2||i%10==3||i%10==9)
    {
    c++;}
    return c;
    
}
int main()
{
    int t,result,n,m;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d",&n,&m);
        result=function(n,m);
        printf("%d",result);
    }
    return 0;
}
