# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n,m=map(int,input().split())
    j=[]
    for i in range(1,n+1):
        j.append(i) 
        
    for i in range(m):
        w,x,y,z=map(int,input().split())
        
        for k in range(x-1,y):
            if w==1:
                j[k]=j[k]+z 
            elif w==2:
                j[k]=j[k]-z 
    a=min(j)
    b=max(j)
    result=b-a 
    print(result)
        
