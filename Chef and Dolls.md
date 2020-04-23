# BASIC
CodeChef Programs at beginner and easy level
try:
    t=int(input())
    while t>0:
        n=int(input())
        a=[]
        while n>0:
            a.append(int(input()))
            n=n-1
        xor=0
        for i in range(len(a)):
            xor=xor^a[i]
        print(xor)
        t=t-1
except:
    pass
