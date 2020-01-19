#include<stdio.h>
int main()
{
    int t,n,r,rev=0;
    scanf("%d",&t);
    for(int i=0;i<t;i++)
    {
        scanf("%d",&n);
        while(n!=0)
        {
          r=n%10;
          rev=rev*10+r;
          n=n/10;
        }
        
        //if(rev==n)
        //printf("wines");
        //else
        //printf("losses");
        
    }
    if(rev==n)
        printf("wines");
        else
        printf("losses");
        
    return 0;
}
