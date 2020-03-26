# BASIC
Hackerearth Programs at beginner and easy level
t=int(input())

for _ in range(t):
    lst=[0]
    n=int(input())
    for i in range(1,n-1):
        if n%i==0:
            lst.append(i)
    a=sum(lst)
    if a==n:
        flag=1
        #print("Yes")
    else:
        flag=0
        #print("No")
        #break
    if flag==1:
        
        print("Yes")
        #break
    else:
        print("No")
            
