#include <stdio.h>
void push()
{
    int n,top=-1;
    int stack[100];
    scanf("%d",&n);
    int x;
    scanf("%d",&x);
    if(top>=n-1)
    printf("Stack is full");
    else
    top++;
    stack[top]=x;
    
}

int main()
{
    push();
    return 0;
}
