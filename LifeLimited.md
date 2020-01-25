#include <stdio.h>
#include<string.h>

void function() {
    int t;
    scanf("%d",&t);
    for(int i=0;i<t;i++)
    {
        char s1[4],s2[4],s3[4];
        int flag=0;
        scanf("%s",s1);
        scanf("%s",s2);
        scanf("%s",s3);
        for(int j=0;j<strlen(s1);j++)
        {
            if(s1[j]=='l')
            {
                if(s2[j]=='l')
                {
                    if(s2[j+1]=='l')
                    {
                        flag=1;
                    }
                }
            }
        }
        for(int j=0;j<strlen(s2);j++)
        {
            if(s2[j]=='l')
            {
                if(s3[j]=='l')
                {
                    if(s3[j+1]=='l')
                    {
                        flag=1;
                    }
                }
            }
        }
        if(flag==1)
        {
            printf("yes\n");
        }
        else
        {
            printf("no\n");
        }
    }
	// your code goes here
	return 0;
}
int main()
{
    function();
    return 0;
}
