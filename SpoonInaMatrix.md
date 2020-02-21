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
    int t,flag=0;
    int spl[5]={'s','p','o','o','n'},spu[5]={'S','P','O','O','N'};
    scanf("%d",&t);
    while(t--)
    {
        int n,m;
        scanf("%d%d",&n,&m);
        //int a[100][100];
        char str[m];
	    int a[n][m];
	    for(int i=0;i<n;i++)
	    {
	        scanf(" %s",str);
	        for(int j=0;j<m;j++)
	        {
	            a[i][j] = str[j];
	        }
	    }
	     for(int i=0;i<n;i++)
	        {
	            int var1=0,var2=0;
	            for(int j=0;j<m;j++)
	            {
	                if(a[i][j]==spl[var1] || a[i][j]==spu[var2])
	                {
	                    var1++;
	                    var2++;
	                }
	                else
	                {
	                    var1=0;
	                    var2=0;
	                }
	                if(var1==5 || var2==5) 
	                {
	                    flag=1;
	                    break;
	                }
	            }
	            if(flag==1) break;
	        }
	       if(flag==0 && n>=5)
	    {
	       for(int i=0;i<n;i++)
	        {
	            int var1=0,var2=0;
	            for(int j=0;j<m;j++)
	            {
	                if(a[j][i]==spl[var1] || a[j][i]==spu[var2])
	                {
	                    var1++;
	                    var2++;
	                }
	                else
	                {
	                    var1=0;
	                    var2=0;
	                }
	                if(var1==5 || var2==5) 
	                {
	                    flag=1;
	                    break;
	                }
	            }
	            if(flag==1) break;
	        } 
	    }
	    if(flag==1) printf("There is a spoon!");
	    else printf("There is indeed no spoon!");
	    printf("\n");
	}
	return 0;
} 
	    
   
