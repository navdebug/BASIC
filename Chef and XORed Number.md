# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n=int(input())
    for j in range(0,n):
        if j^j+1 == n:
            print(j)
