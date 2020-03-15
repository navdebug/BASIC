# BASIC
CodeChef Programs at beginner and easy level
lst=[]
t=int(input())
for i in range(0,t):
    x=int(input())
    for j in range(0,x):
        ele=int(input())
        lst.append(ele)
    y=int(input())
    for k in range(0,y):
        e=int(input())
        lst.append(e)
    lst.sort(reverse=False)
    print(lst)
