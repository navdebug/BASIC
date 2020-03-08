# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main(void) {
	// your code goes here
	int t,n,k,i,j;
	
	scanf("%d",&t);
	for(i=0;i<t;i++)
	{
	      scanf("%d%d",&n,&k);
	      int arr[101],x;
	      for(j=1;j<=n;j++)
	      {
	            scanf("%d",&arr[j]);
	      }
	      int flag=0;
	      for(j=1;j<=n;j++)
	      {
	          if(arr[j]>=k)
	          {
	              x=arr[j]-k;
	              arr[j+1]=arr[j+1]+x;
	          }
	          else
	          {
	              flag=1;
	              break;
	          }
	      }
	      if(flag==0)
	      {
	          printf("YES\n");
	      }
	      else
	      {
	          printf("NO"" %d\n",j);
	      }
	}
	return 0;
}
