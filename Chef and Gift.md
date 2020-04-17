# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    c=0
    n,k=map(int,input().split())
    arr=list(map(int,input().split()))
    for j in range(n):
        if arr[j]%2==0:
            c=c+1 
    if(c==n and k==0):
        print("NO")
    elif(c>=k):
        print("YES")
    else:
        print("NO")
        
    
    
