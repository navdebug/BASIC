# BASIC
CodeChef Programs at beginner and easy level
t = int(input())
for i in range(t):
    n=int(input())
    a=list(map(int,input().split()))
    l=max(a)
    s=min(a)
    for i in range(len(a)):
        if a[i] == s:
            print(s,l)
            break
        if a[i] == l:
            print(l,s)
            break
