#include <stdio.h>
#include <math.h>

int main(void) {
	// your code goes here
    unsigned int n,ans=0;
    scanf("%u",&n);
    char s[n+1];
    scanf("%s",s);
    for(int i=n-1;i>=0;i--){
        if(s[i] == '1'){
            break;
        }
        ans++;
    }
    printf("%u",ans);
	return 0;
}

