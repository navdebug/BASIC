#include <stdio.h>
#include<string.h>

void function()
{
    int t;
    scanf("%d",&t);
    while(t--)
    {
        int n,i,count=0,count1=0;
        scanf("%d",&n);
        char str1[100],str2[100];
        scanf("%s",str1);
        scanf("%s",str2);
        for(i=0;i<n;i++)
        {
            if(str1[i]=='1')
            count++;}
        for(i=0;i<n;i++)
        {if(str2[i]=='1')
            count1++;
            
        }
        if(count==count1)
        printf("YES\n");
        else
        printf("NO\n");
        
    }
    	return 0;
}
int main()
{
    function();
    return 0;
}
