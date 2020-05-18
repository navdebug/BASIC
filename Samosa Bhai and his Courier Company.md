# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
l=[]
for i in range(t):
    l=[0]
    n,k=map(int,input().split())
    arr=[int(i) for i in input().split()]
    for i in range(n):
        for j in range(i+1,n):
            
            a=abs(arr[i]-arr[j])**k 
            l.append(a) 
    e=sum(l)
    print(e)
