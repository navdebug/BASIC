# BASIC
CodeChef Programs at beginner and easy level
for j in range(int(input())):
    n=int(input())
    x=list(map(int,input().split()))
    a=sum(x)
    b=a//(n-1)
    for i in x:
        print(b-i,end=" ")
    print()
