#include <stdio.h>

void function()
{
	// your code goes here
	int t;
	scanf("%d",&t);
	for(int i=0;i<t;i++)
	{
	    int n;
	    scanf("%d",&n);
	    int a[n];
	    for(int j=0;j<n;j++)
	    {
	        scanf("%d",&a[j]);
	    }
	    int sod=0;
	    for(int j=0;j<n-1;j++)
	    {
	        for(int k=j+1;k<n;k++)
	        {
	            int sum=0;
	            int prod=a[j]*a[k];
	            while(prod!=0)
	            {
	                sum+=prod%10;
	                prod=prod/10;
	            }
	            if(sum>sod)
	            {
	                sod=sum;
	            }
	        }
	    }
	    printf("%d\n",sod);
	}
	//return 0;
    
}

int main()
{
    function();
    return 0;
}
