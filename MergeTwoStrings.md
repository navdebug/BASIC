# BASIC
CodeChef Programs at beginner and easy level


#include <stdio.h>
int main()
{
   char s1[100],s2[100];
   scanf("%s%s",s1,s2);
   for(int i=0,j=0;s1[i]!='\0'||s2[j]!='\0';)
   {
       if(s1[i]!='\0')
       printf("%c",s1[i++]);
       if(s2[j]!='\0')
       printf("%c",s2[j++]);
   }
 
    return 0;
}
