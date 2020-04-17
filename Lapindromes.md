# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for j in range(t):
    s=str(input())
    a = len(s)//2
    s1 = s[:a] 
    s2 = list(s[-a:]) 
    for i in s1:
        if i in s2:
            s2.remove(i)
            if len(s2)==0:
                print("Yes")
        else:
            print("No")
            break 
