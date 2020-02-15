# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
#include <stdlib.h>
 
int main(void){
	int t,n,i,j,l, h, k, **a;
	char b[32] = {'\0'};
	scanf("%d", &t);
	
	 while(t--)
	  {
	  scanf("%d", &n);
 
	  a = (int **)malloc(n * sizeof(int *));
	  
		for(i=0;i<n;++i)
		{
			a[i] = (int *)malloc(n * sizeof(int));
		}
 
		for(i=0;i<n;++i)
		{
			for(j=0;j<n;++j)
			{
				scanf("%1d",&a[i][j]);
			}
		}
	  
	  h = n-1;
	  l = 0;
	  k = 0;
	  
	  while(l<=h)
	  {
	    for(i=0,j=n-1;i<=j;i++,j--)
	    {
	       if((a[l][i] != a[l][j]) || (a[h][i] != a[h][j]) || (a[l][i] != a[h][i]) || (a[h][i] != a[l][i]))
	       {
	           k = 1 ;
	           break;
	       }
	    }
	    
	    if(k == 1)
	    {
	        break;
	    }
	  
		l++;
		h--;
	  }
	  if(k == 0)
	  {
	  	printf("YES\n");
	  }
	  else
	  {
	  	printf("NO\n");
	  }
	  free(a);
	}
	
	return 0;
}
