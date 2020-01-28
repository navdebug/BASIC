#include <stdio.h>

void function()
{
	// your code goes here
	int a,b,c;
	scanf("%d %d",&a,&b);
	c=a-b+1;
	if(c%10==0)
	{
	    printf("%d",c-2);
	}
	else
	{
	    printf("%d",c);
	}
	
}
int main()
{
    function();
    return 0;
}
