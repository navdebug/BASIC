# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main(){
	int t;
	scanf("%d",&t);
	while(t--){
	    long int n,i,j,k,a[10000],b[10000],p;
	    scanf("%ld",&n);
	    for(i=0;i<n;i++)
	    scanf("%ld",&a[i]);
	    for(k=0;k<n;k++)
	    {
	        p=1;
	        for(i=0;i<n;i++)
	        {
	            if(i!=k)
	            p=p*a[i];
	        }
	        b[k]=p;
	        
	    }
	    for(i=0;i<n;i++)
	    printf("%ld ",b[i]);
	  printf("\n");
	}
	return 0;
}
