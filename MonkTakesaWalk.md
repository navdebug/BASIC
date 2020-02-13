/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <stdio.h>
#include<string.h>
int compute (char s[100])
{
    int c=0;
    int len;
    len=strlen(s);
    for(int i=0;i<len;i++)
    {
        if(s[i]=='A'||s[i]=='a'||s[i]=='e'||s[i]=='E'||s[i]=='i'||s[i]=='I'||s[i]=='o'||s[i]=='O'||s[i]=='u'||s[i]=='U')
        c++;
    }
    return c;
}

int main()
{
    //printf("Hello World");
    int t;
    char s[100];
    scanf("%d",&t);
    while(t--)
    {
        scanf("%s",s);
        int r=compute(s);
        printf("%d",r);
    }
    return 0;
}
