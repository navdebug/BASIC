# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main(void) {
	int n1,n2,c=0;
	scanf("%d\n",&n1);
	scanf("%d\n",&n2);
	if(n1>n2){
	    c=n1-n2;
	}
	else{
	    c=n1+n2;
	}
	printf("%d\n",c);
	return 0;
}
