# BASIC
CodeChef Programs at beginner and easy level


#include <stdio.h>
#include<string.h>
int main()
{
    int n;
    scanf("%d",&n);
    while(n--)
    {
    int flag=1;
   char s1[100],s2[100];
   scanf("%s%s",s1,s2);
   int len1=strlen(s1);
   int len2=strlen(s2);
   for(int i=0;i<len1;i++)
   {
       for(int j=0;j<len2;j++)
       {
           if(s1[i]==s2[j])
           flag=1;
           else
           flag=0;
       }
   }
   if(flag==1)
   printf("YES");
   else
   printf("NO");
   
    }
    printf("\n");
    return 0;
}
