# BASIC
CodeChef Programs at beginner and easy level
n = int(input())
for _ in range(n):
    s=input()
    c=True
    if s[0]==s[1]:
        c=False
    else:
        for i in range(len(s)-2):
            if s[i]!=s[i+2]:
                c=False
                break
    if c:
        print("YES")
    else:
        print("NO")
