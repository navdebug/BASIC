
#include <stdio.h>

void function() {
	// your code goes here
	int t,i,j,m,n,Rx,Ry,l,x,y;
	char s[10000];
	scanf("%d",&t);
	for(i=0;i<t;i++)
	{
	          x=0;
	          y=0;
	    scanf("%d %d %d %d %d",&m,&n,&Rx,&Ry,&l);
	    scanf("%s",s);
	    for(j=0;j<l;j++)
	    {
	               if(s[j]=='L')
	               x--;
	               else if(s[j]=='R')
	               x++;
	               else if(s[j]=='U')
	               y++;
	               else if(s[j]=='D')
	               y--;
	              
	    }
	    if(x==Rx && y==Ry)
	     printf("Case %d: REACHED\n",i+1);
	    else if(x<0 || x>m || y<0 || y>n)
	     printf("Case %d: DANGER\n",i+1);
	    else
	     printf("Case %d: SOMEWHERE\n",i+1);
	}
	
}
int main()

{
    function();
    return 0;
}


