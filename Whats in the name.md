# BASIC
CodeChef Programs at beginner and easy level
for i in range(int(input())):
    t=list(input().split())
    p=''
    if len(t)==3:
        p+=t[0][0].upper()+'.'+t[1][0].upper()+'.'+t[2][0].upper()+t[2][1:].lower()
    elif len(t)==2:
        p+=t[0][0].upper()+'.'+t[1][0].upper()+t[1][1:].lower()
    else:
        p+=t[0][0].upper()+t[0][1:].lower()
    print(p)
