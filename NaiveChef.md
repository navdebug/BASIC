#include<stdio.h>
int main()
{
    int num;
    scanf("%d",&num);
    while(num--)
    {   
        int N;
        double A,B,k1=0,k2=0,sum;
        scanf("%d %lf %lf",&N,&A,&B);
        double a[N];
        for(int i = 0 ; i < N ; i++)
        scanf("%lf",&a[i]);
        for(int i = 0 ; i < N ; i++)
        {
            if(a[i]==A)
            k1++;
            if(a[i]==B)
            k2++;
        }
        sum=(k1*k2)/(N*N);
        printf("%lf\n",sum);

    }
    return 0;
}
