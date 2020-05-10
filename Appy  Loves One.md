# BASIC
CodeChef Programs at beginner and easy level
from collections import deque
x,y,z=map(int,input().split())
a=list(input().split())
a=a+a
a="".join(a)
n=input()
k=0
r=2*x
l=x
s=deque(a[l:r])
for i in n:
    if i=="!":
        k=s.pop()
        s.appendleft(k)
        #print(s)
    elif i=="?":

        #print(s)
        lol="".join(s)
        lol=int(lol,2)
        yo=0
        while lol>0:
            lol&=lol<<1
            yo+=1
        print(min(yo,z))        
            
            
