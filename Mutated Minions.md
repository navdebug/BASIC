# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n,k=map(int,input().split())
    arr=list(map(int,input().split()))
    c=0
    for i in range(n):
        arr[i]=arr[i]+k 
        if arr[i]%7==0:
            c+=1
    print(c)
