Geeks for Geeks
 #include<stdio.h>
 int main(){
 int a;
    int temp=0;
    scanf("%d",&a);
    while(a--)
    {
         int n,d;
         scanf("%d",&n);
         d=n*n;
        int b[d],arr[n][n];
	    int i,j;
	    for(i=0;i<n;i++)
	    {
	        for(j=0;j<n;j++)
	        {
	        scanf("%d",&arr[i][j]);
	        }
	    }
	    int x=0;
	     for(i=0;i<n;i++)
	    {
	        for(j=0;j<n;j++)
	        {
	        b[x]=arr[i][j];
	        x++;
	        }
	    }
	    for(i=0;i<d;i++)
	    {
	        for(j=0;j<d;j++)
	        {
	            if(b[i]<b[j])
	            {
	                temp=b[i];
	                b[i]=b[j];
	                b[j]=temp;
	            }
	           
	        }
	    }
	    for(i=0;i<d;i++)
	    {
	        printf("%d ",b[i]);

	    }
	    printf("\n");
    }
    
   
	return 0;
}
