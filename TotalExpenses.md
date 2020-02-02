#include <stdio.h>

void function()
{
    int m;
    scanf("%d",&m);
    while(m--){
        double num1,num2,dis;
        scanf("%lf%lf",&num1,&num2);
        if(num1 < 1000)
            printf("%lf\n",(num1 * num2));
        else{
            dis = (num1 * num2) * 0.1;
            printf("%lf\n",((num1 * num2) - dis));
        }
    }
	// your code goes here
	return 0;
}
int main()
{
    function();
    return 0;
}
