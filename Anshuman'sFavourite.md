# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main() {
	int t,n;
	scanf("%d",&t);
	while(t--)
	{
	   	    scanf("%d",&n);
	    if(n%5==0)
	    printf("YES");
	    else
	    printf("NO");
	}
	return 0;
}
