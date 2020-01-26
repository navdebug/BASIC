#include <stdio.h>

int main(void) {
	int t;
	scanf("%d",&t);
	while(t--)
	{
	    int n,i;
	    scanf("%d",&n);
	    char s[n+1];
	    scanf("%s",&s);
	    int cnt=0;
	    for(i=0;i<n-1;++i)
	     {
	         if((s[i]!='a'&& s[i]!='e'&&s[i]!='i' && s[i]!='o' && s[i]!='u')&&(s[i+1]=='a' ||s[i+1]=='e'||s[i+1]=='i'||s[i+1]=='o'||s[i+1]=='u'))
	            cnt++;
	     }
	     
	     printf("%d\n",cnt);
	}
	return 0;
}
