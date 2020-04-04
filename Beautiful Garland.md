# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    s=str(input())
    a=s.count('R')
    b=s.count('G')
    if a==b:
        print("yes")
    else:
        print("no")
