#include<stdio.h>
void function()
{
   
   double a,b;
	char ch;
	scanf("%lf %lf",&a,&b);
	scanf(" %c ",&ch);
	if(ch=='+') 
	    printf("%lf\n",a+b);
	else if(ch=='-') 
	    printf("%lf\n",a-b);
	else if(ch=='*') 
	    printf("%lf\n",a*b);
	else
	    printf("%lf\n",a/b);
	
	return 0;
}
int main()
{
    function();
    return 0;
}
