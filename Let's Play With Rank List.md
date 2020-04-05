# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n,s=map(int,input().split())
    if((n*(n+1))//2==s):
        print(0)
        continue
    elif(n==s):
        print(n-1)
    else:
        var=1
        s=s-n
        while(((var*(var+1))//2)<=s):
            var+=1
        print(n-var)
