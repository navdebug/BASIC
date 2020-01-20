#include <stdio.h>
#include <string.h>
int main()
{
  int i,k,n,c=0,d=0,j;
  char str[100];
  scanf("%d",&k);
  for(i=0;i<k;i++)
  {
    scanf("%s",str);
    n=strlen(str);
    for(j=0;j<n;j++)
     {
       if(str[j]=='a')
       {

       c++;
       }
       else if(str[j]=='b')
       {
          d++;
     }
   }
     if(c>d)
     {
       printf("%d\n",d);
        }
        else printf("%d\n",c);
c=0;
d=0;
    }

    return 0;
}
