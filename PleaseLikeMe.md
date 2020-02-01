#include<stdio.h>
#include<stdlib.h>
void function()
{
	int t;
	scanf("%d",&t);
	while(t--)
	{
		long long int l,d,c,s,sum;
		scanf("%lld %lld %lld %lld",&l,&d,&s,&c);
		sum=s;
			for(int i=0;i<d-1;i++)
			{
				sum=sum+sum*c;
				if(sum>=l)
				break;
			}	
		if(sum<l)
		printf("DEAD AND ROTTING\n");
		else
		printf("ALIVE AND KICKING\n");
	}
}	
int main()
{
    function();
    return 0;
}
