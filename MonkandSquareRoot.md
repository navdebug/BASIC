# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
typedef long long ll;
 
int main()
{
    int test;
    ll n,i,m,ans;
    scanf("%d",&test);
    while(test--)
    {
        scanf("%lld%lld",&n,&m);
        ans=1;
        for(i = 0;i<m;i++)
        {
            if((i*i)%m == n)
            {
                ans = i;
                break;
            }
        }
        printf("%lld\n",ans);
    }
    return 0;
}
