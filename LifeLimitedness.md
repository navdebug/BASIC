# BASIC
CodeChef Programs at beginner and easy level

    #include <stdio.h>

int main(void) {
	// your code goes here
	int t,i,j,flag=1;
	char s[3][3];
	scanf("%d",&t);
	while(t--)
	{
	    
	    for(i=0;i<3;i++)
	    {
	        for(j=0;j<3;j++){
	         scanf(" %c",&s[i][j]);}}
	         for(i =0;i<3;i++)
	         {for(int j=0;j<3;j++){
	       if(s[0][0]=='l'&&s[1][0]=='l'&&s[1][1])
	         flag=0;
	         else
	         flag=1;
	         }
	         }
	    if(flag==1)
	    printf("NO");
	    else
	    printf("YES");
    }
    return 0;
}
