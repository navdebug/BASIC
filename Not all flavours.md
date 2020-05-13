# BASIC
CodeChef Programs at beginner and easy level
def solve():
    (n,k)=(map(int,input().split()))
    a=list(map(int,input().split()))
    
    if k==1:
        print(0)
        return 
    m=0
    j=0
    item=[]
    item.append(a[0])
    for i in range(1,n):
        if a[i] in item:
            continue
        elif len(item)+1 < k:
            item.append(a[i])
        else:
            #print(item,a[i])
            item=[]
            item.append(a[i])
            m=max(m,(i-j))
            j=i
    
    print(max(m,n-j))

t=int(input())
for i in range(t):
    solve()
    
    
        
