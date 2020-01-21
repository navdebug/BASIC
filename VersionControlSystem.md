#include <stdio.h>
void function()
{
    int t,n,m,k,i[100],h[100],bothcount=0,uncount=0;
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d%d%d",&n,&m,&k);
        for(int g=0;g<m;g++)
        scanf("%d",&i[g]);
        for(int r=0;r<k;r++)
      scanf("%d",&h[r]);
      for(int f=0;f<m;f++)
      {
          for(int u=0;u<k;u++)
          {
              if(i[f]==h[u])
              bothcount++;
              
              
          }
      }
      
    }
    uncount= n-(m+k-bothcount);
    printf("%d\n",bothcount);
    printf("%d\n",uncount);
}
int main()
{
 function();
    return 0;
}

