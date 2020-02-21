Chef and Xored Numbered
#include <stdio.h>
int main()
{
  int t;
  scanf("%d",&t);
  while(t--){
      int n,m=0,p=1;
      scanf("%d",&n);
      while(p<=n){
          p=m^(m+1);
          m=p;
      }
      if(n==1)
          printf("2\n");
      else if(p/2 == n)
          printf("%d\n",(p/2)/2);
      else
          printf("-1\n");
      
  }
    return 0;
}
