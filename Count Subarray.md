# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n=int(input())
    l=list(map(int,input().split()))
    s=1
    c=1
    for i in range(1,n):
        if(l[i]>=l[i-1]):
            c+=1
        else:
            c=1
        s=s+c
    print(s)
        
        
