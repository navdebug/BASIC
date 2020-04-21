# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    s1=""
    s=input()
    c=0
    for i in range(len(s)):
        if s[i]!=s1:
            s1=s[i] 
            c+=1 
    print(c//2) 
        
