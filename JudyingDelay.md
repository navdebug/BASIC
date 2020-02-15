#include <stdio.h>

int main(void) {
	int t,n,s,j;
	scanf("%d",&t);
	while(t--){
	    int c=0;
	    scanf("%d",&n);
	    while(n--){
	        scanf("%d %d",&s,&j);
	        if((j-s)>5){
	            c++;
	        }
	    }
	    printf("%d\n",c);
	}
	return 0;
}

