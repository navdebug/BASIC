# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
#include <stdlib.h>
int max(int a,int b)
{
    if(a>b)
    {
        return a;
    }
    else
    {
        return b;
    }
}
int main(void) {
	unsigned int t;
	scanf("%u",&t);
	if(t<1000)
{	
	while(t--)
	{
	    unsigned int s,y;
	    scanf("%u%u",&s,&y);
	    unsigned long int a[s],sum=0,max1=0;
	      for(int i=0;i<s;i++)
	      {
            scanf("%lu",&a[i]);
            sum += a[i];
            max1 = max(max1, a[i]);
         }

        if(sum % y == 0  && max1 <= sum/y)
            printf("YES\n");
        else
            printf("NO\n");
	}
}
	return 0;
}
