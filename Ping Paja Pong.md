# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    x,y,k=map(int,input().split())
    d=(x+y)//k 
    if d%2==0:
        print("Chef")
    else:
        print("Paja")
