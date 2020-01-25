
#include<stdio.h>
#include<string.h>
int main()
{     int j,T;
scanf("%d",&T);
    for(j=1;j<=T;j++)
    {
		int i,flag=0,l;
	    char a[1000];
	scanf(" %[^\n]",a);
	l=strlen(a);
	for(i=0;i<l;i++)
	{
	 	if(a[i]==' ' && a[i+1]=='n' && a[i+2]=='o' && a[i+3]=='t' && a[i+4]==' ')
	 	{
	 		flag=1;
	 		break;
		 }
		 else if(a[i]==' ' && a[i+1]=='n' && a[i+2]=='o' && a[i+3]=='t' && a[i+4]=='\0')
		 {
		 	flag=1;
		 	break;
		 }
		 else if(a[0]=='n' && a[1]=='o' && a[2]=='t' && a[3]==' ')
		 {
		 	flag=1;
		 	break;
		 }
		 else if(a[0]=='n' && a[1]=='o' && a[2]=='t' && a[3]=='\0')
		 	 {
		 	flag=1;
		 	break;
		 }
		  else continue;
	}
	if(flag==1)
	printf("Real Fancy");
	else
	printf("regularly fancy");
	printf("\n");
    }
	return 0;
}
