# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n,k=map(int,input().split())
    arr=list(map(int,input().split()))
    for i in range(n):
        if arr[i]==k or arr[i]>=k:
            flag=1
            break
        else:
            flag=0 
    if flag ==1:
        print("Yes")
    else:
        print("No")
