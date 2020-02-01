#include<stdio.h>
void function()
{
    int t,n,output;
    while(t--)
    {
       scanf("%d",&n);
       int a[n];
       for(int i=0;i<n;i++)
       {
       scanf("%d",&a[i]);
       }
       for(int j=0;j<n;j++)
       
       {
           for(int u=1;u<=a[j]&&u<=a[j+1];u++)
           {
               if(a[j]%u==0&&a[j+1]%u==0)
               output=u;
           }
           
       }
       printf("%d",output);
    }
}
int main()


{
    function();
    return 0;
}
