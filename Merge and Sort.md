# BASIC
CodeChef Programs at beginner and easy level
lst=[]
n=int(input())
for i in range(0,n):
    ele=int(input())
    lst.append(ele)
m=int(input())
for j in range(0,m):
    e=int(input())
    lst.append(e)
lst.sort(reverse=False)
print(lst)
