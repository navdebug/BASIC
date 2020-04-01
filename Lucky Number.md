# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for _ in range(t):
    n,a,b=map(int,input().split())
    A=list(map(int,input().split()))
    cnta=0
    cntb=0
    cnt=0
    for i in range(n):
        if(A[i]%a==0 and A[i]%b==0):
            cnt=1
        elif(A[i]%a==0):
            cnta+=1
        elif(A[i]%b==0):
            cntb+=1
    cntb=cntb-cnt
    if(cnta>cntb):
        print("BOB")
    else:
        print("ALICE")
