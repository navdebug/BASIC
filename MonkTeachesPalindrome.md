#include<stdio.h>
#include<string.h>
void function(char s[100])
{
   char b[100];
   strcpy(b,s);
   strrev(b);
   if(strcmp(s,b)==0)
   {
       
       int len=strlen(s);
       if(len%2==0)
         printf("YES EVEN");
         else
         printf("YES ODD");
   }
   
   else
   printf("NO");
   
    
}
int main()
{
    int t;
    char s[100];
    scanf("%d",&t);
    while(t--)
    {
        scanf("%d",s);
        function(s);   
    }
    return 0;
}
