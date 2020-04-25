# BASIC
CodeChef Programs at beginner and easy level
n=int(input())
x=int(input())
for i in range(n+1):
    s=pow(2,i)
    if(x%s!=0):
        t=i
        break
print(t-1)
