# BASIC
CodeChef Programs at beginner and easy level
for i in range(int(input())):
    n=int(input())
    r=input().split()
    arr=[]
    for j in range(n):
        arr.append(int(r[j]))
    c2=0
    c=0
    for j in range(n):
        if arr[j]==2:
            c2+=1
        if arr[j]>2:
            c+=1
    ans=c2*c + c*(c-1)//2
    print(ans)
