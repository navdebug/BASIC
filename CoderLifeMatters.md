#include<stdio.h>
int main()
{
    int i,a[30],t,count;
    int flag;
    scanf("%d",&t);
    while(t--)
    {
        count=0;
        flag=0;
        for(i=0;i<30;i++)
        {
            scanf("%d",&a[i]);
        }
        for(i=0;i<30;i++)
        {
            if(a[i])
            {
                count++;
                if(count>5)
                {
                    flag=1;
                    break;
                }
            }
            else
            {
                count=0;
            }
        }
        if(flag)
            printf("#coderlifematters\n");
        else
            printf("#allcodersarefun\n");
    }
    return 0;
}
