    #include <stdio.h>
     
    int main(){
        
        int t,n,k, j;
        scanf("%d",&t);
        int arr[100000];
        
        for (int i = 0;i<t;i++){
            scanf("%d %d",&n,&k);
            for (j = 0;j<n;j++){
                scanf("%d",arr+j);
            }
            k %= n;
            for (j = n-k;j<n;j++){
                printf("%d ",arr[j]);
            }
            for (j = 0;j<n-k;j++){
                printf("%d ",arr[j]);
            }
            putchar('\n');
        }
        
        return 0;
    }
