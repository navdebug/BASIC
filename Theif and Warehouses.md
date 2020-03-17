# BASIC
CodeChef Programs at beginner and easy level


    #include<stdio.h>
    int main()
    {
       long long int i,j,k,t,n;
       scanf("%lld",&t);
       while(t--)
       {
           scanf("%lld",&n);
           long long arr[n],sum=0,max=0;
           for(i=0;i<n;i++)
           scanf("%lld",&arr[i]);
           for(i=0;i<n;i++)
           {
                 sum=0;
            for(j=i;j<n;j++)
            { 
                if(arr[j]<arr[i])
                    break;
                else
                    sum=sum+arr[i];
                
            }
            for(k=i-1;k>=0;k--)
            {
                if(arr[k]<arr[i])
                    break;
                else
                    sum=sum+arr[i];
            }
            if(sum>max)
                max=sum;
           }
           printf("%lld\n",max);
       }
       return 0;
    }


