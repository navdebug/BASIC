# BASIC
Hackerank Programs at beginner and easy level

INPUT 
1
3 2
1 2 3

OUTPUT 
1

for i in range(int(input())):
    n,m=map(int,input().split())
    a=list(map(int,input().split()))
    l=[]
    for i in range(n+1):
        for j in range(i,n+1):
            s=a[i:j]
            e=sum(s)
            f=e%m 
            l.append(f)
    print(max(l))
            
    
    

