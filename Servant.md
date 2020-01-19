#include<stdio.h>
int main()
{
    int t,n;
    scanf("%d",&t);
    for(int i=0;i<t;i++)
    {
        scanf("%d",&n);
        if(n<10)
        printf("What an obedient servant you are");
        else
        printf("%d",-1);
    }
    
    return 0;
}
