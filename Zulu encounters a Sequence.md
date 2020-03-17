# BASIC
Hackerearth Programs at beginner and easy level
t =int(input())
lst=[]
for i in range(0,t):
    n=int(input())
    for i in range(0,n):
        ele=int(input())
        lst.append(ele)
    a=max(lst)
    b=min(lst)
    c=abs(a-b)
    print(c)
    
        
