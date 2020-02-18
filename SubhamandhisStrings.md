# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
#include<string.h>
 
int main(void)
{
    int t,n,i;
    char a[100001];
    int count,k;
    char temp;
    scanf("%d",&t);
    for(int p=0;p<t;p++)
    {
        count=0;
        scanf("%d",&n);
        scanf("%s",&a);
        for(i=0;i<n;i++)
        {
            if(a[i]=='0')
            {
                count++;
            }
        }
        printf("%d\n",count);
    }
}
