# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
#include<stdlib.h>
#include<math.h>
int main()
{
  long int t;
  scanf("%ld",&t);
  while(t>0)
  {
     long long int i,j,k,s,n,u,p,y,ca;
     s=0;
     scanf("%lld",&n);
     u=0;
     y=0;
     while(1)
     {
       p=sqrt(y);
       p++;
       y=y+p*p;
       u++;
       if(y>=n*n)
       {
          break;
       }
      }
      printf("%lld\n",u);
      t--;
  }
}
