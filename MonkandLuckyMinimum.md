#include<stdio.h>
int main()
{
    int a[100],b[100],c=0,n,min=10000;
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    scanf("%d",&a[i]);
    for(int g=0;g<n;g++)
    {
        if(a[g]<min)
        min=a[g];
    }
    //printf("%d",min);
    for(int j=0;j<n;j++)
    {
        if(a[j]==min)
        {
            c++;
        }
    }
    //printf("%d",c);
    if(c%2==0)
    printf("Unlucky");
    else
    printf("lucky");
    
    
    return 0;
}
