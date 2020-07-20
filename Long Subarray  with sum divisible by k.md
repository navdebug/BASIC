# BASIC
CodeChef Programs at beginner and easy level
INPUT 
6 3
2 5 6 1 4 5

OUTPUT 
4

n,k=map(int,input().split())
arr=list(map(int,input().split())) 
m=0 
l=[]
for i in range(n+1):
    for j in range(i,n+1):
        s=arr[i:j]
        d=sum(s)
        if d%k==0:
            l.append(len(s))  
print(max(l))
            
