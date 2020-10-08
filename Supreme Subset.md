from itertools import combinations 
n,m=input().split()
n,m=int(n),int(m)
arr=list(map(int,input().split()))
c=0   
g=[]
e=list(combinations(arr,2)) 
for i in e:
    if (i[1]-i[0])%m==0:
        c+=1 
        g.append(i)    
print(c)
ans=10000
for i in g:
    ans=min(ans,(i[1]+i[0])) 
for j in g:
    if (j[1]+j[0])==ans: 
        print(j[0],j[1],sep=" ")
    
