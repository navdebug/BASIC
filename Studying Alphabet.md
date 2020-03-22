# BASIC
CodeChef Programs at beginner and easy level
s = input()
list1 = []
n = int(input())
for i in range(n):
    flag = 1
    w = input()
    for item in w:
        if item not in s:
            flag = 0
    if(flag==1):
        list1.append("Yes")
    elif(flag==0):
        list1.append("No")

for items in list1:
    print(items)
