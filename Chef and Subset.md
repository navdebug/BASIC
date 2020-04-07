# BASIC
CodeChef Programs at beginner and easy level
from itertools import combinations 
for i in range(int(input())):
    a=list(map(int,input().split()))
    if a.count(0)>0:
        print("Yes")
    else:
        if sum(a)==0:
            print("Yes")
        else:
            a.sort()
            b=list(combinations(a,2))
            c=list()
            for j in b:
                c.append(sum(j))
            d=list(combinations(a,3))
            e=list()
            for j in d:
                e.append(sum(j))
            if c.count(0)>0 or e.count(0)>0:
                print("Yes")
            else:
                print("No")
