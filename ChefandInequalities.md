# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main(void) {
	// your code goes here
	int t;
	scanf("%d",&t);
	while(t--){
	long long int a,b,c,d,count=0;
	scanf("%llu %llu %llu %llu",&a,&b,&c,&d);
	for(int i=a;i<=b;i++)
	{if(i<c)
	 {count=count+d-c+1;}
	 else if(i<d)
	 {count=count+d-i;}}
	printf("%llu\n",count);
	}
	return 0;
}
