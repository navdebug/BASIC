# BASIC
CodeChef Programs at beginner and easy level
for j in range(int(input())):
    n,k=map(int,input().split())
    f=input()
    x=list(f)
    c,d=0,0
    for i in x:
        if(i==i.upper()):
            c+=1
        elif(i==i.lower()):
            d+=1
    if(c<=k and d<=k):
        print("both")
    elif(c<=k):
        print("chef")
    elif(d<=k):
        print("brother")
    else:
        print("none")
