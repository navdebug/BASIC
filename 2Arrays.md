# BASIC
CodeChef Programs at beginner and easy level
#include<stdio.h>
void main(){
int n,c1=0,c2=0,s1=0,s2=0;
scanf("%d",&n);
int a[n],b[n];
for(int i=0;i<n;i++)
scanf("%d",&a[i]);
printf("\n");
for(int i=0;i<n;i++)
scanf("%d",&b[i]);
for(int i=0;i<n;i++){
if(a[i]==-1)
c1++;
else
s1=s1+a[i];
if(b[i]==-1)
c2++;
else
s2=s2+b[i];
}
if(c1==c2)
printf("Infinite\n");
else if(c1==1||c2==1)
{ if(c1==1&&s1>s2)
printf("0\n");
else if(c2==1&&s2>s1)
printf("0\n");
else
printf("1\n");}
else
{ if(c1==2&&s1>s2)
printf("0\n");
else if(c2==2&&s2>s1)
printf("0\n");
else{
int d=abs(s1-s2);
if(s1==s2)
printf("1\n");
else
printf("%d\n",d+1);
}}
}
