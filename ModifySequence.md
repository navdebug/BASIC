# BASIC
CodeChef Programs at beginner and easy level
    #include <stdio.h>
    int main()
    {
        int n,i;
        long int arr[100000];
        scanf("%d",&n);
        for(i=0;i<n;i++)
        {
            scanf("%ld",&arr[i]);
        }
        for(i=1;i<n;i++)
        {
            arr[i]=arr[i]-arr[i-1];
        }
        if(arr[n-1]==0)
        printf("YES\n");
        else
        printf("NO\n");
    }
