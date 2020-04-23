# BASIC
CodeChef Programs at beginner and easy level
for i in range(int(input())):
    n,k=map(int,input().split())
    l=list(map(int,input().split()))
    l.sort() 
    a=l[(n+k)//2]
    print(a)
