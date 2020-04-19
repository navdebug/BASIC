# BASIC
CodeChef Programs at beginner and easy level
T=int(input())
lis1=[]
lis2=[]
for i in range(T):
    N=int(input())
    lis1=list(map(int,input().strip().split()))[:N]
    lis2=list(map(int,input().strip().split()))[:N]
    lis3=[]
    lis3.append(lis1[0])
    count=0
    for j in range(len(lis1)-1):
        lis3.append(lis1[j+1]-lis1[j])
    for x in range(len(lis2)):
        if lis3[x]>=lis2[x]:
            count+=1
        else:
            continue
    print(count)
