# BASIC
CodeChef Programs at beginner and easy level

#include <stdio.h>
#include<string.h>
//int main()

 int main()
{
	int t;
	scanf("%d",&t);
	while(t!=0)
	{
		int n,i,j,flag,arr[100],brr[100]={0};
		scanf("%d",&n);
		for(i=0;i<n;i++)
			scanf("%d",&arr[i]);
		for(i=0;i<n;i++)
		{
			if(brr[i]==0)
			{
				flag=0;
				for(j=i+1;j<n;j++)
				{
					if(arr[i]==arr[j])
					{
						brr[j]=1;
						flag=1;
					}
				}
				if(flag==0)
				{
					printf("%d",arr[i]);
					break;
				}
			}				
		}
		if(flag==1)
			printf("0");
		printf("\n");
		t--;
	}
return 0;
}
