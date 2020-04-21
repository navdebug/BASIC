# BASIC
CodeChef Programs at beginner and easy level
c=0
n=int(input())
for i in range(n):
    s=input()
    if "ch" in s or "he" in s or "ef" in s:
        c=c+1
print(c)
