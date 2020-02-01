#include <stdio.h>
#include <stdbool.h>
void function()
{
    // your code goes here
    int t = 0, i=1,g,q=1,n;
    scanf("%d", &t);
    while (t--)
    {
        scanf("%d",&g);
        while(g--)
        {
            scanf("%d%d%d",&i,&n,&q);
            
            if(n%2==0)
            printf("%d",n/2);
            else
            {
                if(i==q)
                {
                printf("%d",n/2);
                }
                else
                {
                    printf("%d",n/2+1);
                }
                
            }
        }
    }
}
int main()
{
    function();
    return 0;

}
            
            
            
