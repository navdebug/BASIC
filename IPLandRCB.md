
#include <stdio.h>

int main(void) {
	int T,X,Y;
	scanf("%d",&T);
	while(T)
	{
	    scanf("%d %d",&X,&Y);
	    if(X<=Y)
	    {
	        printf("\n 0");
	    }
	    else
	    {
	        printf("\n %d",X-Y);
	    }
	    T--;
	}// your code goes here
	return 0;
}

