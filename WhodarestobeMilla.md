int main(void)
{
	int t,max;
	scanf("%d",&t);
	while(t--)
	{
	    int n,i,count=0;
	    scanf("%d",&n);
	    char corr[n];
	    char ans[n];
	    int arr[n+1];
	    scanf("%s",corr);
	    scanf("%s",ans);
	    for(i=0;i<=n;i++)
	    {
	        scanf("%d",&arr[i]);
	    }
	    for(i=0;i<=n-1;i++)
        {

           if(ans[i]==corr[i])
           {
           	   count++;
           }
        }
        max=arr[count];
        if(count!=n)
        {
            for(i=0;i<=count;i++)
            {
        	if(arr[i]>max)
        	  max=arr[i];
            }
        }
        
        printf("%d\n",max);


    }
	return 0;
}
