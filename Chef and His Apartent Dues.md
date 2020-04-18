# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n=int(input())
    l = list(map(int,input().split()))
    p=n*1000
    q=0
    for i in range(len(l)):
        if(l[i]==0):
            q=q+1
        else:
            p=p-1000
            if(q!=0):
                q=q+1
            
    print(p+q*100)  
