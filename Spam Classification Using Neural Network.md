# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n,minA,maxA=list(map(int, input().split()))
    a=maxA-minA+1 
    c=a//2
    x=minA%2
    y=1
    for i in range(n):
        w,b=list(map(int, input().split()))
        w=w%2
        b=b%2
        if w==0:
            y=0
        if x==0 or w==0:
            x=b 
        elif b==0:
            x=1 
        else:
            x=0
    if x==0:
            if y==0:
                print(a, end=' ')
                print(0)
            else:
                print(a-c, end=' ')
                print(c)
    else:
        if y==0:
            print(0, end=' ')
            print(a)
        else:
            print(c, end=' ')
            print(a-c)
