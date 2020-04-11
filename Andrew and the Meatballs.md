# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n,m=map(int,input().split())
    a=list(map(int,input().split()))
    s=sum(a)
    a=sorted(a)
    if s<m:
        print(-1)
    else:
        i=n-1
        c=0
        sumn=0
        while(sumn<m):
            sumn+=a[i]
            i=i-1 
            c+=1 
        print(c)
