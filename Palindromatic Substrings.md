# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    s=str(input())
    s1=str(input())
    flag=0
    for j in s:
        if j in s1:
            flag=1 
            break 
    if flag==0:
        print("No")
    elif flag==1:
        print("Yes")
            
