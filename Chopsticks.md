# BASIC
CodeChef Programs at beginner and easy level
n,d=map(int,input().split())
l=[]
for i in range(n):
    l.append(int(input()))
l.sort()

c=0
j=0
while j< (n-1):
    
    if l[j+1]-l[j]<=d:
        c=c+1
        j=j+2
    else:
        j=j+1
print(c)
