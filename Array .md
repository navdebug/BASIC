# BASIC
G Programs at beginner and easy level
n=int(input())
arr=list(map(int,input().split()))
a=sum(arr)
if a%2==0 and a%3==0 and a%5==0:
    print("1")
else:
    print("0")
    
