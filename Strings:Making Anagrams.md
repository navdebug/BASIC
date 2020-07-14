# BASIC
Hackerrank Programs at beginner and easy level

INPUT 
abs
sde

OUTPUT 
4


from math import fabs
def fun(a,b):
    l=[0]*26
    for i in a:
        index=ord(i)-ord('a')
        l[index]+=1 
    for j in b:
        index=ord(j)-ord('a')
        l[index]-=1 
    re=0 
    for j in l:
        re+= fabs(j)
    return re
    
    
    
a=input()
b=input()
print(fun(a,b))
