#include <stdio.h>

int main() {
    int m=0,c=0,x=0,y=0,n=0,a=0,p=0,p1=0,p2=0;
    scanf("%d\n",&n);
    scanf("%d%d\n",&m,&c);
	while(n--){
	    scanf("%d %d %d\n",&x,&y,&p);
	    a=y-(m*x)-c;
	    if(a>0)
	        p1=p1+p;
	        else
	        p2=p2+p;
	}
	if(p1>p2)
printf("%d",p1);
else
printf("%d",p2);

return 0;
}
