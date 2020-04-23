# BASIC
CodeChef Programs at beginner and easy level
for i in range(int(input())):
    n=int,input().split()
    l=list(map(int,input().split()))
    j=set(l)
    c=0
    for k in j:
        if c<l.count(k):
            c=l.count(k)
    if c==0:
        print(0)
    else:
        print(len(l)-c)
            
   
