#include <stdio.h>

long long int a[10005];
char opr[4];
int main(void) {
	// your code goes here
	long long int i,k,m,t,ans,n;
	
	scanf("%lld", &t);
	while(t--)
	{
	    scanf("%lld %lld %lld", &n,&k,&ans);
	    for(i=0;i<n;i++)
	    scanf("%lld",&a[i]);
	    scanf("%s", opr);
	   
	    if(opr[0]=='X')
	    {
	        
	        if(k!=0&&k%2!=0)
	        {
	            
	            for(i=0;i<n;i++)
	            {
	                ans=ans^a[i];
	            }
	            
	            
	            
	        }
	        
	    }
	    
	    else if(opr[0]=='O')
	    {
	        
	        if(k!=0)
	        {
	            for(i=0;i<n;i++)
	            {
              ans=ans|a[i];
	            }
	           
	            
	        }
	        
	    }
	    
	    else if(opr[0]=='A')
	    {
	        if(k!=0 && ans!=0)
	        {
	            for(i=0;i<n;i++)
	            {
	                ans=ans&a[i];
	            }
	            
	            
	        }
	        
	        
	    }
	    
	    printf("%lld\n",ans);
	    
	}
	return 0;
}

