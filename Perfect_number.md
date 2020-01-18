

#include <stdio.h>

 main()
{
    
    int n,sum=0,i=1;
    printf("Enter a perfect number");
    scanf("%d",&n);
    while(n%i==0)
    {
        sum=sum+i;
        i++;
    }
    if(sum==n)
    printf("Entered number is perfect number");
    else
    printf("Entered number is not perfect number");
    //return 0;
}
    
    

