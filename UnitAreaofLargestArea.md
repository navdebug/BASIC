# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main()
{
    int t,c=0;
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
        for(int y=0;y<n;y++)
        {
            for(int l=0;l<m;l++)
            {
                if(a[y][l]==1)
                c++;
            }
        }
       printf("%d",c);
       
    }
    return 0;
}
