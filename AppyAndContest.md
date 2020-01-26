#include<stdio.h>
void function()
{
    int t,n,a,b,k,appy,chef,countappy=0,countchef=0,output;
    scanf("%d",&t);
    
    while(t--)
    {
        scanf("%d%d%d%d",&n,&a,&b,&k);
        for(int i=0;i<n;i++)
        {
            if(n%a==0)
            {
                countappy++;
            }
            else if(n%b==0)
            {
                countchef++;
            }
        output=countappy+countchef;
        //if(output>=k)
        //printf("win");
        //else
        //printf("loss");
        }
        if(output>=k)
        printf("win");
        else
        printf("loss");
        
    }
}
int main()
{
    function();
    return 0;

}
