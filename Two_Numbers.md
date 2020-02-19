# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main(void) {
	int t;
	scanf("%d",&t);
	while(t--)
	{
	    long int a,b,n;
	    scanf("%ld%ld%ld",&a,&b,&n);
	    long int min,max;
	    if(a>=b)
	      { max=a;
	        min=b;
	      }
	      
	    else
	      {
	          max=b;
	          min=a;
	      }
	      
	      if(n%2==0)
	        printf("%ld\n",max/min);
	        
	      else
	        {
	            if((2*a)>=max)
	              {
	                  max=2*a;
	                  min=b;
	                  printf("%ld\n",max/min);
	              }
	              
	             else
	               {
	                   max=b;
	                   min=2*a;
	                   printf("%ld\n",max/min);
	               }
	        }
	        
	}
	return 0;
}
