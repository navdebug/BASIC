# BASIC
CodeChef Programs at beginner and easy level
n = int(input())
a = list(input())
b = [] 
for i in range(n):
    if(i==0 or len(b)==0):
        b.append(a[i])
    elif(a[i]==b[len(b)-1]):
        b.pop()
    else:
        b.append(a[i])

print("".join(b)) 

n=int(input()) 
string=list(input()) 
stack=[]
[stack.pop() if stack and stack[-1]==i else stack.append(i) for i in string]
print(len(stack),"".join(stack),sep="\n")


