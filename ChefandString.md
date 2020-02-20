# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main(void) {
    char s[100001];
    scanf("%s",&s);
    int p=0,a=0,b=0,c=0;
    for(int i=0;s[i]!='\0';i++) {
        if(s[i]=='C') {
            a++;
        }
        else if(s[i]=='H' && a>=b+1) {
            b++;
        }
        else if(s[i] == 'E' && b>=c+1) {
            c++;
        }
        else if(s[i] == 'F' && c>=p+1) {
            p++;
        }
    }
    printf("%d",p);
	
	return 0;
}
