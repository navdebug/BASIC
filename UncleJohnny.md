#include <stdio.h>
void function()
{
	int n,k,t,i,val,temp,j;
	scanf("%d",&t);
	while(t--)
	{
	    scanf("%d",&n);
	    int arr[n];
	    for(i=1;i<=n;i++)
	    {
	        scanf("%d",&arr[i]);
	    }
	    scanf("%d",&k);
	    val=arr[k];
	    printf("%d",val);
	}
}
int main()
{
    function();
    return 0;
}
