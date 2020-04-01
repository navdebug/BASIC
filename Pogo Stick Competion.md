# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n,k=map(int,input().split())
    arr=list(map(int,input().split()))
    ans=[0]*n
    for i in range(n-1,-1,-1):
        ans[i]=arr[i]
        if i+k<n:
            ans[i]+=ans[i+k]    
    print(max(ans))
