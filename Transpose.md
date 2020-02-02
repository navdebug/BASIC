#include<stdio.h>
void function()
{
    int m,n;
    scanf("%d%d",&m,&n);
    int a[m][n],b[10][10],c[m][n];
    for(int i=0;i<m;i++)
    {
        for(int j=0;j<n;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
    for(int i=0;i<m;i++)
    {
        for(int j=0;j<n;j++)
        {
            
            b[j][i]=a[i][j];
        }
    }
    for(int i=0;i<n;i++)
    {
        for(int j=0;j<m;j++)
        {
           printf("%d",b[i][j]);
        }
    }
    
}
int main()
{
    function();
    return 0;
}

