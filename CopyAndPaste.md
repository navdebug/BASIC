#include <stdio.h>
#include <string.h>

#define MAX 100001

void function()
{
    int t, n, x, count, i;
    scanf("%d", &t);

    while (t--) {
        scanf("%d", &n);
        int f[MAX] = {0};
        for (i = count = 0; i < n; i++) {
            scanf("%d", &x);

            if (!f[x]) {
                f[x] = 1;
                count++;
            }
        }

        printf("%d\n", count);
    }

    return 0;
}
int main()
{
    function();
    return 0;
}
