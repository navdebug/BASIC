# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
lst=[]
lst1=[]
minimum=99999
for i in range(0,t):
    n,m,k=list(map(int,input().split()))
    if m>n and k==1:
        n+=k 
        print(m-n)
    elif n>m and k==1:
        m+=k 
        print(abs(m-n))
    elif k!=1:
        t1=max(n,m)-min(n,m)
        if(t1>k):
            print(t1-k)
        else:
            print("0")
