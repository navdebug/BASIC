# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int gcd(long long int a,long long int b)
{
    long long int c = a,temp;
	while(b)
	{
		temp = a%b;
		a = b;
		b = temp;
	}
	if(a!=1 && a!= c)
		return 1;
	return 0;
}
int main()
{
	long long int n,num,count=0,i;
	scanf("%lld",&n);
	while(n--)
	{
		count =0;
		scanf("%lld",&num);
		for(i=2;i<num;i++)
		{
			if(gcd(i,num))
				count++;
		}
		printf("%lld\n",count);
		
	}
	return 0;
}
