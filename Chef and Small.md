# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n,k=map(int,input().split())# n and money 
    app=[]
    for i in range(n): 
        cost,weight=map(int,input().split())
        app.append([cost,weight])
    app.sort()
    sm= 0 
    cnt= 0
    for i in range(n):
        curr=app[i][0]
        if curr+sm <=k:
            cnt+=1 
            sm+=curr 
    print(cnt)
