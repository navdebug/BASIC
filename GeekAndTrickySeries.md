# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main() {
	int t;
	scanf("%d",&t);
	
	while(t--)
	{
	    int n;
	    scanf("%d",&n);
	    if(n<=0)
     {
         return -1;
     }
    long arr[122];
    arr[0]=7;
    for(int i=1;i<122;i++)
    {
         arr[i]=(arr[i-1]*2+i)%1000000007;
    }
    printf("%d",arr[n-1]);
	}
}
