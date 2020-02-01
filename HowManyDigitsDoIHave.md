#include <stdio.h>

 void function() 
{
	// your code goes here
	int n;
	scanf("%d",&n);
	if(n>0&&n<10)
	printf("1\n");
	else if(n>9&&n<100)
	printf("2\n");
	else if(n>99&&n<1000)
	printf("3\n");
	else
	printf("More than 3 digits\n");
	return 0;
}
int main()
{
    function();
    return 0;
}
