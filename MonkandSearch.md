# BASIC
CodeChef Programs at beginner and easy level
/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <stdio.h>

int main()
{
    int n,a[100],c=0;
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    int q;
    scanf("%d",&q);
    while(q--)
    {
        int x,y;
        scanf("%d%d",&x,&y);
        if(x==0)
        {
            for(int i=0;i<n;i++)
            if(a[i]>=y)
            c++;
            else
            c=0;
        }
        else if(x==1)
        {
            for(int i=0;i<n;i++)
            if(a[i]>y)
            c++;
            else
            c=0;
        }
        printf("%d",c);
    }

    return 0;
}
