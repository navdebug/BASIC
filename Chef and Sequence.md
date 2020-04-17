# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n=int(input())
    flag=0
    arr=list(map(int,input().split()))
    f=int(input())
    arr1=list(map(int,input().split()))
    for i in arr1:
        if i in arr:
            flag=1
        else:
            flag=0 
    if flag==1:
        print("Yes")
    else:
        print("No")
        break
    
