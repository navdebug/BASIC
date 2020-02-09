#include<stdio.h>
void function(int a,int b,int c)
{
    
    
   if (a<=b&&b<=c || a>=b&&b>=c)
            printf("%d\n",b);
       else if(b<=a&&a<=c || b>=a&&a>=c)
            printf("%d\n",a);
        else 
            printf("%d\n",c);
    
    
    
}
int main()
{
    int t,a,b,c,result;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d%d",&a,&b,&c);
        function(a,b,c);
        //printf("%d",result);
    }
}
