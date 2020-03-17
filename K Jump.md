# BASIC
CodeChef Programs at beginner and easy level
k=int(input())
n=int(input())
count=0
lst=[]
for i in range(0,n):
    ele=int(input())
    lst.append(ele)
for i in range(0,n):
    for j in range(i+1,n):
        if(lst[j]-lst[i]>=k):
            count=count+1 
        else:
            count=0
print(count)
