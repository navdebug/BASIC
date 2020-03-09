# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
int main()
{
    int n,c=0;
    scanf("%d",&n);
    int bin[32];
    int i=0;
    while(n!=0)
    {
        bin[i]=n%2;
        n=n/2;
        i++;
    }
    for(int j=0;j<32;j++)
    {
        if(bin[j]==1)
        c++;
        
    }
    printf("%d",c-1);
    
}
