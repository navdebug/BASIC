# BASIC
Hackearth Programs at beginner and easy level
n=int(input())
lst=[]
sub=[[]]
for _ in range(0,n):
    e=int(input())
    lst.append(e)
for i in range(n+1):
    for j in range(i,n+1):
        s=lst[i:j]
        sub.append(s)
print(sub)
    
