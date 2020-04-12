# BASIC
CodeChef Programs at beginner and easy level
try:
    t=int(input())
    for _ in range(t):
        n=int(input())
        s=p=su=0
        l=list(map(int,input().split()))[:n]
        s=l.count(2)
        p=l.count(5)
        for i in l:
            if(i>=2 or i<=5):
                su=su+i 
            else:
                su=0
        if(su==0 or (su/n)<4):
            print("No")
        elif(s==0 and p>=1 and (su/n)>=4):
            print("Yes")
except:
    pass
