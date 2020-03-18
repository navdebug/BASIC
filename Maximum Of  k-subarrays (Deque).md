# BASIC
CodeChef Programs at beginner and easy level
n,k=map(int,input().split())
lst=[]
sub=[[]]
dum=[]
for r in range(n):
    ele=int(input())
    lst.append(ele)
for i in range(n+1):
    for j in range(i,n+1):
        s=lst[i:j]
        if len(s)==k:
            sub.append(s)
            dum.append(max(s))
print(dum)
