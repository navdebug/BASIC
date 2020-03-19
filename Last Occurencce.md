# BASIC
Hackerearth Programs at beginner and easy level


#include <stdio.h>

int main()
{
    int n,m;
    scanf("%d%d",&n,&m);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for (int t=n;t>=0;t--)
    {
        if(a[t]==m){
        printf("%d",t+1);
        break;}
    }
    
    return 0;
}

