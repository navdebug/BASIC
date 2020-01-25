#include<stdio.h>
#include<string.h>

#define ll long long int 

int main()
{

 ll t;
 scanf("%lld",&t);
 while(t!=0)
 {
  ll w,i,j;
  char s[8];
  scanf("%lld",&w);
  scanf("%s",s);
  ll count[7];
  
  for(i=0;i<7;i++)
  count[i]=4;
  
  
   if(w%7==1)
  {
   if(!strcmp(s, "mon"))
   count[0]++;
   if(!strcmp(s, "tues"))
   count[1]++;
   if(!strcmp(s, "wed"))
   count[2]++;
   if(!strcmp(s, "thurs"))
   count[3]++;
   if(!strcmp(s, "fri"))
   count[4]++;
   if(!strcmp(s,  "sat"))
   count[5]++;
   if(!strcmp(s,"sun"))
   count[6]++;
   }
   
   else if(w%7==2)
  {
   if(!strcmp(s, "mon"))
   { count[0]++,count[1]++;}
   if(!strcmp(s, "tues"))
  { count[1]++,count[2]++;}
   if(!strcmp(s, "wed"))
   { count[2]++,count[3]++;}
   if(!strcmp(s, "thurs"))
    { count[3]++,count[4]++;}
   if(!strcmp(s, "fri"))
   { count[4]++,count[5]++;}
   if(!strcmp(s,  "sat"))
   { count[5]++,count[6]++;}
   if(!strcmp(s,"sun"))
   { count[6]++,count[0]++;}
   }
   
   else if(w%7==3)
  {
   if(!strcmp(s, "mon"))
  { count[0]++,count[1]++,count[2]++;}
   if(!strcmp(s, "tues"))
   { count[3]++,count[1]++,count[2]++;}
   if(!strcmp(s, "wed"))
   { count[3]++,count[4]++,count[2]++;}
   if(!strcmp(s, "thurs"))
   { count[3]++,count[4]++,count[5]++;}
   if(!strcmp(s, "fri"))
   { count[4]++,count[5]++,count[6]++;}
   if(!strcmp(s,  "sat"))
   { count[5]++,count[6]++,count[0]++;}
   if(!strcmp(s,"sun"))
   { count[6]++,count[1]++,count[0]++;}
   }
 
   for(i=0;i<7;i++)
   printf("%lld\t",count[i]);
   printf("\n");
   t--;
   
 }
}
   
  
  
 
