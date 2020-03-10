# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main()
{
    int t,c=0,swap;
    scanf("%d",&t);
    while(t--)
    {
        int n;
        scanf("%d",&n);
        int a[n];
        for(int i=0;i<n;i++)
        {
            scanf("%d",&a[i]);
        }
        for(int j=0;j<n-1;j++)
        {
            for(int d=0;d<n-j-1;d++)
            {
                if (a[d]>a[d+1]) 
                {
                    swap=a[d];
                    a[d]=a[d+1];
                    a[d+1]=swap;
                    c++;
                }
            }
        }
        printf("%d",c);
    }
    return 0;
}
                
