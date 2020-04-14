# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n=int(input())
    l=list(map(int,input().split()))
    s=sum(l)
    if(s/n in l):
        print(l.index(s//n)+1)
    else:
        print("Impossible")
