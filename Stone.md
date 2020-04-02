# BASIC
CodeChef Programs at beginner and easy level
N,k=map(int,input().split())
l=list(map(int,input().split()))
l1=[]
l2=[]
maxi=max(l)
mini=min(l)
for i in range(len(l)):
    l1.append(maxi-l[i])
    l2.append(l[i]-mini)
if(k==0):
    print(*l)
elif(k!=0 and k%2==0):
    print(*l2)
else:
    print(*l1)
    
    
