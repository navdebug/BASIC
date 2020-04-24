# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    l,b=map(int,input().split())
    m=0
    n=0
    for i in range(l+b+1):
        m=(m+(2*i)+1)
        n=(n+(2*i)+2)
        if(m>l):
            print("Bob")
            break
        elif(n>b):
            print("Limak")
            break
