# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    s=input()
    sum=0
    for l in s:
        if l.isdigit():
            sum=sum+int(l)
    print(sum)
