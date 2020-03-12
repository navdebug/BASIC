# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>

int main()
{
    int t,p=0;
    scanf("%d",&t);
    while(t--)
    {
        int n,m;
        scanf("%d%d",&n,&m);
        int a[n][m];
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<m;j++)
            {
                scanf("%d",&a[i][j]);
            }
        }
        for(int r=0;r<n;r++)
        {
            for(int c=0;c<m;c++)
            {
                if(a[r][c]==2)
                {
                     a[r-1][c]=2;
                     a[r+1][c]=2;
                     a[r][c-1]=2;
                     a[r][c+1]=2;
                     //p++;
                }
            }
        }
        for(int e=0;e<n;e++)
        {
            for(int t=0;t<m;t++)
            {
                printf("%d\t",a[e][t]);
            }
        }
        printf("%d",p);
    }
    return 0;
}
