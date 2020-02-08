# include <stdio.h>
# include <stdlib.h>
int main()
{
	long long  int s,arr[100000];
	int n,i,a,temp,index;;
	scanf("%d",&n);
	while(n--)
	{
		s=0;
		scanf("%d",&a);
		for(i=0;i<a;i++)
		scanf("%lld",arr+i);
		temp=arr[0];
		index=0;
		for(i=1;i<a;i++)
			if(arr[i]<temp)
			{
		temp=arr[i];
		index=i;
			}
		for(i=0;i<a;i++)
		if (i!=index)
		s+=(arr[i]*temp);
		printf("%lld\n",s);
		}
	}
