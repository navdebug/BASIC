#include <stdio.h>
int main(void) {
	// your code goes here
	int t,i;
	scanf("%d",&t);
	while(t--)
	{
	    int d,c=0;
	    float p=0,a=0;
	    scanf("%d",&d);
	    char s[d];
	    scanf("%s",s);
	    for(i=0;i<d;i++)
	    {
	       if(s[i]=='P')
	            {
	                p++;
	            }
	    }
	    a=p/d;
	    for(i=2;(i<d-2)&&(a<0.75);i++)
	       {
	           if((s[i]=='A')&&(s[i-1]=='P'||s[i-2]=='P')&&(s[i+1]=='P'||s[i+2]=='P'))
	           {
	               p++;
	               c++;
	               a=p/d;
	           }
	       }
	       if(a>=0.75)
	            printf("%d\n",c);
	       else
	            printf("-1\n");
	}
	return 0;
}

