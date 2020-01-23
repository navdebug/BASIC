include <stdio.h>
#include <stdlib.h>

int main(){
    long long int t,i,a,b,count = 0;
    scanf("%lld",&t);
    while(t--){
        scanf("%lld %lld",&a, &b);
        if(a % 2 == 0 && b % 2 == 0){
            count = (b-a)/2;
        }
        else{
            count = ((b-a)/2) + 1;
        }
    
        if(count % 2 == 0){
            printf("Even\n");
        }
        else{
            printf("Odd\n");
        }
    }
    return 0;
    
}
