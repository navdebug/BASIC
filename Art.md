#include <stdio.h>
#include <stdlib.h>

int main(void) {
	int T,N,Cn2,Cn1,Cn,valid;
	scanf("%d\n",&T);
	while (T--) {
	    valid=0;
	    scanf("%d\n",&N);
	    Cn2=-1; Cn1=-1; Cn=-1;
	    while (N--) {
	        Cn2=Cn1; Cn1=Cn;
	        scanf("%d",&Cn);
	        if (Cn2==Cn1 && Cn1==Cn) valid=1;
	    }
	    if (valid==1) printf("Yes\n");
	    else printf("No\n");
	}
	return 0;
}

