# BASIC
CodeChef Programs at beginner and easy level
#include <stdio.h>
int main()
{
    int t;
    int sum;
    scanf("%d",&t);
    while(t--)
    {
        sum=0;
        int n;
        scanf("%d",&n);
        int a[n];
        for(int i =0;i<n;i++)
        scanf("%d",&a[i]);
        int lst[n];
        if (a[0]==0){
            for (int l=0;l<n;l++)
            lst[l]=a[l+1];
        }
        else
        {
            lst[0]=a[0];
        }
        
        int k=1;
        for (int j =1;j<n;j++)
        {
            if (a[j]!=0)
            {
            lst[j]=a[j]-k;
            k++;}
            else{
                lst[j]=a[j];
                k++;
            }
        }
        for (int u=0;u<n;u++){
            
            sum=sum+lst[u];
        }
        printf("%d",sum);
    
        
    }
    return 0;
}
