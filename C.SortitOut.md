# BASIC
CodeChef Programs at beginner and easy level


#include <stdio.h>

int main()
{
    int n,temp;
    int a[100],b[100];
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    {scanf("%d",&a[i]);
    b[i]=i;
    }
    for(int j=0;j<n;j++)
    {
        for(int t=0;t<n-1-j;t++)
        {
            if(a[t]<a[t+1])
            temp=a[t];
            a[t]=a[t+1];
            a[t+1]=temp;
            temp=b[t];
            b[t]=b[t+1];
            b[t+1]=temp;
        }
    }
    for(int i=0;i<n;i++)
    printf("%d\t",b[i]);
    return 0;
}
   
