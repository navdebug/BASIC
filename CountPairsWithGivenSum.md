From GeeksforGeeks

#include <stdio.h>
#include<string.h>
int main()

   {
    int T,sum,c=0;
    scanf("%d",&T);
    while(T--)
    {
      int n,k;
      scanf("%d%d",&n,&k);
      int a[n];
      for(int i=0;i<n;i++)
      {
          scanf("%d",&a[i]);
      }
      for(int i=0;i<n;i++)
      {
          for(int j=i+1;j<n;j++)
          {
              sum=a[i]+a[j];
              if(sum==k){
              c++;}
          }
      }
      printf("%d",c);
    }
	return 0;
}
