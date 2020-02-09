#include<stdio.h>
#include<string.h>
int main()
{
    int i,a;
    scanf("%d",&a);
    for(i=0;i<a;i++)
    {
        int j=0,b=0,c=0,d=0;
        char s[100];
        scanf("%s",s);
        b=strlen(s);
       while(j<b-1)
        {
            if(s[j]=='m'&&s[j+1]=='s')
            {
            s[j+1]=' ';
            j=j+2;
            }
            else if(s[j]=='s'&&s[j+1]=='m')
            {
            s[j]=' ';
            j=j+2;
            }
           else
           j=j+1;
       }
        for(j=0;j<b;j++)
       {
         if(s[j]=='m')
         c=c+1;
         else if(s[j]=='s')
         d=d+1;
         
        }
        if(c>d)
        printf("mongooses\n");
        else if(d>c)
        printf("snakes\n");
        else
        printf("tie\n");
    }
}
