
n,q=map(int,input().split())
flag=0
arr=[int(i) for i in input().split()]
for j in range(q):
        
    l,r,k=map(int,input().split())
    for i in range(l,r):
        e=arr.count(arr[l])
        if e>=k:
            flag=arr[l]
        else:
            flag=0 
    if flag==0:
        print(-1)
    else:
        print(flag)
