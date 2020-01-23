#include <stdio.h>
int main(void)
{
	int t;
	scanf("%d",&t);
	for(int k=1;k<=t;k++)
	{
	    int m,n,c=0;
	    scanf("%d %d",&m,&n);
	    int arr[m],brr[n];
	    for(int i=0;i<m;i++)
	    {
	        scanf("%d",&arr[i]);
	    }
	    for(int i=0;i<n;i++)
	    {
	        scanf("%d",&brr[i]);
	    }
	    for(int i=0;i<m;i++)
    	{
    	    for(int j=0;j<n;j++)
    	    {
    	       if(arr[i]==brr[j])
    	           c++;
    	    }
	    }
	    printf("%d\n",c);
    }
	return 0;
}



