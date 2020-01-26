#include<stdio.h>
void function()
{
	int t, n, a[50], i;
	char pl[5];
	scanf("%d",&t);
	while(t--)
	{
		scanf("%d %s",&n, pl);
		for(i=0;i<n;i++)
			scanf("%d",&a[i]);
		if(n==1 && a[0]%2==0 && pl[1]=='e')
			printf("Dee\n");
		else printf("Dum\n");
	}
	return 0;
}
int main()
{
    function();
    return 0;
}
 
