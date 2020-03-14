# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
int main(){
	int n;
	scanf("%d", &n); 
	int A[n],B[n],i,j;
	int sum1=0,sum2=0;
	
	for(i=0;i<n;i++)
	{
	    scanf("%d",&A[i]);
	    
	    if(A[i]!=-1)
	    sum1=sum1+A[i];
	}
	for(i=0;i<n;i++)
	{
	    scanf("%d",&B[i]);
	    
	    if(B[i]!=-1)
	    sum2=sum2+B[i];
	}
	   
 
	  
	
	int d1=0,d2=0;
	
	for(i=0;i<n;i++)
	{
	    if(A[i]==-1)
	    d1++;
	}
	
	for(i=0;i<n;i++)
	{
	    if(B[i]==-1)
	    d2++;
	}
	
 
	 if(d1==1&&d2==1)
	 printf("Infinite\n");
	 
	 else
	 {
	  
	   if(d1==1||d2==1)
	   {
	       if(sum2>=sum1&&d1==1)
	       printf("%d\n",1);
	       else if(sum1>=sum2&&d2==1)
	       printf("%d\n",1);
	       else
	       printf("%d\n",0);
	   }
	   else
	   {
	       if(sum2==sum1)
	       printf("%d\n",1);
	       else
	       {
	           if(sum2>sum1&&d1==2)
	           printf("%d\n",sum2-sum1+1);
	           else if(sum2<sum1&&d2==2)
	           printf("%d\n",sum1-sum2+1);
	           else
	           printf("%d\n",0);
	       }
	   }
	   
	 }
	return 0;
}
