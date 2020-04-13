# BASIC
CodeChef Programs at beginner and easy level
# cook your dish here
def grade(a,b,c):
    if(a>50 and b<0.7 and c>5600):
        print(10)
    elif(a>50 and b<0.7):
        print(9)
    elif(b<0.7 and c>5600):
        print(8)
    elif(a>50 and c>5600):
        print(7)
    elif(a>50 or b<0.7 or c>5600):
        print(6)
    else:
        print(5)
   
test=int(input())
for i in range(test):
    n,m,k=map(float,input().split(" "))
    grade(n,m,k)
