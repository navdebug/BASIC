#include<stdio.h>
#include <string.h>
void function()
{
    int t,count=0;
    char j[10];
    char s[10];
    scanf("%d",&t);
    while(t--)
    {
        scanf("%s",j);
        scanf("%s",s);
    for(int i=0;i<strlen(j);i++)
    {
        for(int y=0;y<strlen(s);y++)
        {
            if(j[i]==s[y])
            count++;
        }
    }
    printf("%d",count);
}}
int main()
{
    function();
    return 0;
}
