#include<stdio.h>
int main()
{
    int t,n,k;
    scanf("%d",&t);
    for(int i=0;i<t;i++)
    {
      scanf("%d%d",&n,&k);
      printf("%d",(n+k));
    }
    return 0;
}
