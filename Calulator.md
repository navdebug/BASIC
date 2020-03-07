# BASIC
CodeChef Programs at beginner and easy level
/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/


    #include <stdio.h>

int main()
{
int t;
scanf("%d",&t);
while(t--)
{
long long int n,i,s=0,b,c=0,k;
scanf("%lld %lld",&n,&b);
s=n/2;

i=s/b;
k=i+1;
c=(n-i*b)*(i);
printf("%d",c);
s=(n-k*b)*(k);

if(c>s) printf("%lld\n",c);
else printf("%lld\n",s);
}
}


   
