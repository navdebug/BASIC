#include <stdio.h>

void function( )
{
    int t;
    scanf("%d",&t);
    while(t--) {
        int n,k;
        scanf("%d%d",&n,&k);
        int a[n];
        int i,f;
        for(i=0;i<n;i++) {
            a[i]=i+1;
            //printf("%d",a[i]);
        }
        
        int temp;
        temp=a[k];
        a[k]=a[n-1];
        a[n-1]=temp;
        for(i=0;i<n;i++) {
        printf("%d ",a[i]);
        }
    }
	return 0;
}
int main()
{
    function();
    return 0;
}

