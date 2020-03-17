# BASIC
CodeChef Programs at beginner and easy level
# cook your dish here
p,r=list(map(int,input().split()))

l=list(map(int,input().split()))
l.sort()
a=min(l[0],l[-1])
b=max(l[0],l[-1])
for _ in range(r):
    n=int(input())
    if(a<=n and n<=b):
        print('Yes')
    else:
        print('No')
