# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n,k=map(int,input().split())
    arr=[int(i) for i in input().split()]
    while k>0:
        arr.remove(min(arr))
        arr.remove(max(arr))
        k=k-1 
    a=sum(arr)/len(arr)
    print(a)
        
        
        
        
