# BASIC
CodeChef Programs at beginner and easy level
for x in range(int(input())):
    a,b=map(str,input().split())
    if len(a)==len(b)==2:
        r=int(b[1])*10+int(b[0])*10+int(a[0])+int(a[1])
        k= int(a[1])*10+int(a[0])*10+int(b[0])+int(b[1])
        p= int(a)+int(b)
        print(max(k,r,p))
    elif len(a)==1 and len(b)==2:
        p= int(a)+int(b)
        k= int(a[0])*10+int(b[1])+int(b[0])
        print(max(p,k))
    elif len(b)==1 and len(a)==2:
        p= int(a)+int(b)
        k= int(b[0])*10+int(a[1])+int(a[0])
        print(max(p,k))
    else:
        print(int(a)+int(b))
