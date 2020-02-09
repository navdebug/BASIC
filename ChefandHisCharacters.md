#include<stdio.h>
#include<string.h>
int main()
 {
     int t;
	scanf("%d",&t);
	while(t--)
	{
	   	char s[5000000];
	     int i=0,j=0,c=0,k=0;
	     int cc=0,ch=0,ce=0,cf=0;
		scanf("%s",s);
		i=0;c=0;
		while(s[i]!=0){
		    cc=ch=ce=cf=0;
			j=0;
			k=i;
			while(j<4){
			    
				if(s[k]=='c')
					cc++;
				else if(s[k]=='h')
					ch++;
				else if(s[k]=='e')
					ce++;
				else if(s[k]=='f')
					cf++;	
				k++;
				j++;
			}
			
			
			i++;
			if(cc==1 && ch==1 && ce==1 && cf==1)
				c=c+1;
		}
		
		if(c>0)
			printf("lovely %d\n",c);
			
		else
			printf("normal\n");
		
			
	}
}
			
