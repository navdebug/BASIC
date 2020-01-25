#include <stdio.h>
#include <string.h>
int main(void) {
	// your code goes here
	int t,i,j,k,l;
	char s1[100][100],s2[100][100];
	scanf("%d",&t);
	for(i=0;i<t;i++)
	{
	          for(j=0;j<4;j++)
	           scanf("%s",s1[j]);
	           for(k=0;k<4;k++)
	            scanf("%s",s2[k]);
	           l=0;
	          for(j=0;j<4;j++)
	          {
	                    for(k=0;k<4;k++)
	                    {
	                              if(strcmp(s1[j],s2[k])==0)
	                               l++;
	                    }
	          }
	         // printf("%d    ",l);
	          if(l>=2)
	           printf("similar\n");
	          else
	           printf("dissimilar\n");
	}
	return 0;
}
