#include<stdio.h>
//void quicksort(unsigned long [105],int,int);
int main()
{
	int t,i;
	scanf("%d",&t);
	while(t--)
	{
		int k,n,j,temp=0;
		scanf("%d %d",&n,&k);
		int w[n],sum=0,total=0;
		
		
//		quicksort(w,0,n-1);
		for(i=0;i<n;i++){
			for(j=i+1;j<n;j++)
			{
				if(w[i]>w[j]){
					temp=w[j];
					w[j]=w[i];
					w[i]=temp;
				}
			}
		}
		
		for(int i=0;i<n;i++)
		printf("%d",w[i]);
	}
}

		
