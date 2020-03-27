# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    b=[]
    sub=[[0]]
    r=[0]
    n,k=map(int, input().split())
    arr=list(map(int,input().split()))
    #for i in arr:
    while k>=-1:
        for i in arr:
            b.append(i)
            k=k-1
    for i in range(len(b)+1):
        for j in range(i,len(b)+1):
            
            s=b[i:j]
            sub.append(s)

    for i in sub:
        #r=[0]
        r.append(sum(i))
    e=max(r)
    print(e)
