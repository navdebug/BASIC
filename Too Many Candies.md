# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n,m,k=map(int,input().split())
    x=n//m 
    y=m*x
    z=n-y
    out=z//k
    print(out)
    
