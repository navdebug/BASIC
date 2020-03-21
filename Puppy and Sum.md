# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(0,t):
    s=0
    d,n=list(map(int,input().split()))
    if d==1 :
        for j in range(1,n+1):
            s=s+j 
    else:
        while d>0:
            for k in range(1,n+1):
                s=s+k 
            
            n=s
            n=n-1
            d-=1
    print(s)
