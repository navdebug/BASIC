# BASIC
CodeChef Programs at beginner and easy level
int main()
{
	int t;
	scanf("%d",&t);
	while(t--){
		int n,rem,sum=0;
	scanf("%d",&n);
	while(n>0)
	{
		while(n!=0)
		{
		rem=n%10;
		sum=sum+rem;
		n=n/10;
	    }
		if(sum > 9)
                 {
                        n = sum;
                        sum = 0;
                 }
	}
	printf("%d\n",sum);
}

	return 0;
}
