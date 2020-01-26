#include <stdio.h>
int main()
{
    int t;
    long long int a, b,p, n;
    scanf("%d", &t);
    while(t--)
    {
        scanf("%lld %lld %lld", &a, &b, &n);
        if(n%2==0)
        {
            if(a>b)
            { p=a/b;
                printf("%lld\n", p);}
            else
                { p=b/a;
                    printf("%lld\n", p);}
        }
        else
        {
            a=a*2;
            if (a>b){ p=a/b;
                printf("%lld\n", p);}
            else {p=b/a;
                printf("%lld\n", p);}
        }
    }
    return 0;
}
