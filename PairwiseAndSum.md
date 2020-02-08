#include <stdio.h>

int main(void) 
{
    int i,j;
    int n,s=0;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++) scanf("%d",&a[i]);
    for(i=0;i<n;i++)
    {
        for(j=n-1;j>i;j--)
           s=s+(a[i]&a[j]);
    }
    printf("%d",s);
	return 0;
}

