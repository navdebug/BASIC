# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n,k=map(int,input().split())
    arr=list(map(int,input().split()))
    arr.append(k)
    a=max(arr)
    for i in range(n):
        if a in arr:
            arr.remove(a) 
     
    e=max(arr)
    print(e)
    
