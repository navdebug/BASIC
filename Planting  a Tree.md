# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for _ in range(t):
    n=input()
    lis=list(map(int,input().split()))
    lis.sort()
    count=0
    for i in lis:
        if (( i+1 in lis )  or  (i-1 in lis)):
            x=0
        else:
            lis.append(i+1)
            count=count+1 
    print(count)
        
