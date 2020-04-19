# BASIC
CodeChef Programs at beginner and easy level
a=int(input())
for i in range(a):
    b=input()
    b+=b[0]
    count=0
    for j in range(len(b)-1):
        if b[j+1]!=b[j]:
            count+=1
    if count<=2:
        print("uniform")
    else:
        print("non-uniform")
