#include<stdio.h>

void function(){
    int T; scanf("%d", &T);
    while (T--) {
        int N, B;
        scanf("%d%d", &N, &B);
        int W, H, P;
        int maxS = 0;
        int found = 0;

        for (int i = 1; i <= N; ++i) {
            scanf("%d%d%d", &W, &H, &P);
            if (W * H >= maxS && P <= B) {
                maxS = W * H;
                found = 1;
            }
        }

        if (!found) printf("no tablet\n");
        else printf("%d\n", maxS);
    }
    return 0;
}
int main()

{
    function();
    return 0;
}
