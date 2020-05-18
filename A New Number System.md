# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
#include<string.h>
int main()
{   int flag=1,k,j;
    char st[35];
     unsigned long num=0;
    while(1)
    {    scanf("%s",&st);     
          
              if(st[0]=='#')
              {
                printf("%lu\n",num);
                num=0;
                continue;
               }
                else if(st[0]=='~')return 0;
          k=strlen(st);    
    
     
      if(k==1)flag=1;
      if(k==2)flag=0;
      else  for(j=0;j<k-2;j++)num=num*2 +flag;
    
}
 
return 0;
}        
     
