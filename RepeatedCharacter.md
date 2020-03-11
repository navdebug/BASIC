# BASIC
CodeChef Programs at beginner and easy level

#include <stdio.h>
#include<string.h>
int main()

   {
    int T ;
    scanf("%d",&T);
    while(T--)
    {
        char arr[100] ;
        int flag = 1 , terminate = 0 ;
        scanf("%s",arr);
        for(int i = 0 ; arr[i]!= '\0' ; i ++)
        {
            for(int j = i + 1 ; arr[j]!='\0' ; j++)
            {
                if(arr[i]==arr[j])
                {
                    printf("%c\n",arr[i]);
                    terminate = 1 ;
                    flag = 0 ;
                    break;
                }
            }
            if(terminate)
            break;
        }
        if(flag)
        printf("-1\n");
    }
	return 0;
}
