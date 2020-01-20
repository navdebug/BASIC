#include <stdio.h>

int main(void) {
	
	int n,a,evencount=0,oddcount=0;
	scanf("%d",&n);
	while(n--)
	{
	    scanf("%d",&a);
	    if(a%2==0)
	    {
	        evencount++;
	    }
	    else
	    {
	        oddcount++;
	    }
	}
	if(evencount>oddcount)
	{
	    printf("READY FOR BATTLE\n");
	}
	else
	{
	    printf("NOT READY\n");
	}
	return 0;
}

