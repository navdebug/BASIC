#include<stdio.h>
void function()
{
    int t,x,y,gcd;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d",&x,&y);
        for(int i=1;i<=x&&i<=y;i++)
        {
            
            
            if(x%i==0&&y%i==0)
            {
               gcd=i; 
            }
        }
        printf("%d",2*gcd);
    }
}

int main(){
    function();
    return 0;
}
