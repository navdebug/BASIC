#include<stdio.h>
int main(void) {
	// your code goes her2
	long long int t,n,a[1001],s,i,j,temp;
	scanf("%lld",&t);
	while(t--)
	{
	    s=0;
	    scanf("%d",&n);
	    for(i=0;i<n;i++)
	    {
	        scanf("%lld",&a[i]);
	    }
	    a[n]=0;
	    if(n==1)
	    printf("%lld\n",a[0]);
	    else if(n==2)
	    printf("%lld\n",a[0]+a[1]);
	    else
	    {
	    for(i=0;i<n;i++)
	    {
	        for(j=0;j<n-1-i;j++)
	        {
	            if(a[j]<a[j+1])
	            {
	                temp=a[j];
	                a[j]=a[j+1];
	                a[j+1]=temp;
	            }
	        }
	    }
	    for(i=0;i<n;i=i+4)
	    {
	        s=s+a[i]+a[i+1];
	    }
	    printf("%lld\n",s);
	    }
	}
	return 0;
}

