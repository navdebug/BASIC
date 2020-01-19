#include<stdio.h>
int main()
{
    int t,temp,n,r,a,s[100],dig=0,count=0;
    scanf("%d",&t);
    
    for(int i=0;i<t;i++)
    {
        scanf("%d",&n);
        temp=n;
        while(temp!=0)
        {
            r=temp%10;
            dig++;
            temp=temp/10;
        
            
        }
        temp=n;
        int a[dig];
        for(int c=dig-1;c>=0;c--)
        {
            r=temp%10;
            temp=temp/10;
            a[c]=r;
        
            if(a[c]==4)
            {
               count=count+1; 
            }
            
        }
        
    printf("%d",count);
    }
    //printf("%d",count);
}
