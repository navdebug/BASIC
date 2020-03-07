# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main()
{
    long long int a[1000001],i,n,l,r,sum=0;
    for(i=0;i<1000000;i++)
       a[i]=i+1;
           scanf("%lld",&n);
       while(n--)
       {
           scanf("%lld %lld",&l,&r);
           if(a[l-1]!=0||a[r-1]!=0)
           for(i=l-1;i<r;i++)
           {
               a[i]=0;
           }
       }
       for(i=0;i<1000000;i++)
       {
           sum+=a[i];
       }
       printf("%lld",sum);
       return 0;
}
