#include<stdio.h>
int main()
{
    int t,n=7,d;
    scanf("%d",&d);
    int arr[]={1,2,3,4,5,6,7};
    
    while(d--)
    {
        int j;
        int temp=arr[0];
        for( j=0;j<n-1;j++)
        arr[j]=arr[j+1];
        arr[j]=temp;
        
    }
    for(int i=0;i<n;i++)
    printf("%d",arr[i]);
}
