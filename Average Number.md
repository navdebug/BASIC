# BASIC
CodeChef Programs at beginner and easy level
for i in range(int(input())):
    a,b,c=map(int,input().split())
    l=list(map(int,input().split()))
    k=(a+b)*c
    j=sum(l)
    m=k-j
    if(m/b>0):
        if(m/b==int(m/b)):
            print(m//b)
        else:
            print(-1)
    else:
        print(-1)
