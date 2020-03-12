Geeks for   Geeks
#include<stdio.h>
int main()
{
int x,t;
scanf("%d",&t);
for(x=0;x<t;x++)
{
    int n,num,i,j,k,f=0;
    scanf("%d",&n);
    scanf("%d",&num);
        int arr[n];
for(i=0;i<n;i++)
{
    scanf("%d",&arr[i]);
}
f=0;
for(j=0;j<n-2;j++)
{
    for(k=j+1;k<n-1;k++)
    {
        for(i=k+1;i<n;i++)
        {
            if(arr[i]+arr[j]+arr[k]==num)
            f=1;
        }
    }
}   


if(f==1)
    printf("1\n");
            else
            printf("0\n");
       
}
	return 0;
}
