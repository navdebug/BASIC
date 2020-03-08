# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main() {
	//code
	int t,gcd;
	scanf("%d",&t);
	while(t--)
	{
	    int n;
	    scanf("%d",&n);
	    for(int i=1;i<n;i++)
	    {
	        if(n%i==0)
	        gcd=i;
	    }
	    if(2*n>=gcd+n)
	    printf("1");
	    else
	    printf("0");
	}
}
