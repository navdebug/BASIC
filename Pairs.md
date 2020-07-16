# BASIC
Hackerrank Programs at beginner and easy level

INPUT 
5 2
1 5 3 4 2

OUTPUT 
3

from itertools import permutations
n,m=map(int,input().split())
a=[int(i) for i in input().split()]
c=0
e=list(permutations(a,2))
p=len(e)
for i in e:
    f=i[0]-i[1]
    if f==m:
        c+=1 
print(c)
    

