# BASIC
Hackerearth Programs at beginner and easy level
import numpy as np
t=int(input())
d=0
for i in range(0,t):
    n=int(input())
    a=list(map(int,input().split()))
    sub=[[]]
    for h in range(0,n+1):
        for y in range(h,n+1):
            s=a[h:y]
            if sum(s)==np.prod(s):
                d+=1 
    print(d)
            
