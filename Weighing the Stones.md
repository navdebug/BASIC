# Hackerearth Programs at beginner and easy level
t =int(input())
lst=[]
lst1=[]
for i in range(0,t):
    n=int(input())
    for i in range(0,n):
        ele=int(input())
        lst.append(ele)
        sum1=0
        sum1=sum(lst)
    for j in range(0,n):
        e=int(input())
        lst1.append(e)
        sum2=0
        sum2=sum(lst1)
    if sum1>sum2:
        print("Rupam")
    elif sum2>sum1:
        print("Ankit")
    else:
        print("Tie")
    
        
