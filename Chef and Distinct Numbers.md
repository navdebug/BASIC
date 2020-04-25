# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
while t:
    t-=1
    n=int(input())
    l=[int(x) for x in input().split()]
    g=set(l)
    if len(g)==n:
        print("No")
        continue
    print("Yes")
