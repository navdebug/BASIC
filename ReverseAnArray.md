# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>

int main()
{
int N;
scanf("%d",&N);
int A[N];
for(int i=0; i<N; i++)
{
scanf("%d",&A[i]);
}
for (int i=N-1; i>=0; i--)
{
printf("%d\n",A[i]);
}
//printf("Hello World!\n");
return 0;
}
