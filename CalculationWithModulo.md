# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
#include<math.h>

int main()
{
	int a,b,c,m;
	scanf("%d%d%d%d", &a,&b,&c,&m);              			// Reading input from STDIN
    int powder=pow(a,b);
    int y=powder/c;
    int z=y%m;
    printf("%d",z);
       // Writing output to STDOUT
}
