#include <stdio.h>
void function()
{
    int t,temp=0;
    scanf("%d",&t);
    int n,k,sum=0,total=0;
    while(t--)
    {
        scanf("%d%d",&n,&k);
        int a[n];
        for(int i=0;i<n;i++)
        {
            scanf("%d",&a[i]);
        }
        for(int l=0;l<n;l++)
        {
            total+=a[l];
        }
        for(int i=0;i<n;i++)
        {
            for(int y=i+1;y<n;y++)
            {
                if(a[i]>a[y])
                temp=a[y];
                a[y]=a[i];
                a[i]=temp;
            }
        }
        
        for(int p=0;p<k;p++)
        {
            sum=sum+a[p];
            total=total-2*sum;
            
        }
        for(int i=0;i<n;i++)
        {
            for(int y=i+1;y<n;y++)
            {
                if(a[i]==a[y])
               {
                   total=(n-k)/2;
                       
                       
                   }
               } 
               
            }
        }
        printf("%d",total);
    }

int main()
{
   function();

    return 0;
}
