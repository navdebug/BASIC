/* C program to print hollow rectangle star pattern */
#include <stdio.h>

/* Function to print hollow rectangle*/
void hollow_rectangle(int n, int m)
{
int i, j;
for (i = 1; i <= n; i++)
{
for (j = 1; j <= m; j++)
{
if (i==1 || i==n || j==1 || j==m)
printf(“*”);
else
printf(” “);
}
printf(“\n”);
}

}

int main()
{
int rows, columns;
printf(“\nEnter the number of rows : “);
scanf(“%d”, &rows);
printf(“\nEnter the number of columns : “);
scanf(“%d”, &columns);
printf(“\n”);
hollow_rectangle(rows, columns);
return 0;
}
