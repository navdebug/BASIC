# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n=int(input())
    arr=list(map(int,input().split()))
    
    lst=[]
    sub=[]
    for i in range(n+1):
        for j in range(i,n):
            x=arr[i]
            
            #print(x)
            lst.append(arr[j]^x)
            #print(lst)
        a=sum(lst)
        sub.append(a)
        
    print(min(sub))
    
