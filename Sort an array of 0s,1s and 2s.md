# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
int main()
{
    int t,swap;
    scanf("%d",&t);
    while(t--)
    {
        int n;
        scanf("%d",&n);
        int a[n];
        for(int i=0;i<n;i++)
        scanf("%d",&a[i]);
        for(int c=0;c<n-1;c++)
        {
            for(int d=0;d<n-c-1;d++)
            {
                if(a[d]>a[d+1])
            {
                swap=a[d];
                a[d]=a[d+1];
                a[d+1]=swap;
            }
            }
        }
        for(int r=0;r<n;r++)
        printf("%d",a[r]);
    }

    return 0;
}
