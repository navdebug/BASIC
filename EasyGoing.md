# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
 
int main(){
	int t,n,m,i,j,k,l,o;
	scanf("%d", &t);              			// Reading input from STDIN
 
    while(t--){
        int diff = 0,minSum = 0,maxSum = 0,maxminD = 0;
        scanf("%d %d",&n,&m);
        
        int A[n];
        
        diff = n - m;
        for(i=0;i<n;i++)
            scanf("%d",&A[i]);
        
        for(j=0;j<n-1;j++){
            for(k=0;k<n-j-1;k++){
                if(A[k]>A[k+1]){
                    int temp;
                    temp = A[k];
                    A[k] = A[k+1];
                    A[k+1] = temp;
                }
            }
        }
        
        for(l=0;l<diff;l++){
            minSum = minSum + A[l];
            
        }
        
        for(o=n-1;o>n-1-diff;o--){
         
                 maxSum = maxSum + A[o];
            
            }
        
            
        maxminD = maxSum - minSum;
        
        printf("%d\n",maxminD);
    }
    return 0;
}
