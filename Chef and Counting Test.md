# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    s=str(input())
    s=list(s)
    e=len(s)
    count=0
    for i in range(e+1):
        for j in range(i,e+1):
            d=s[i:j] 
            if len(d)==2 and d[0]==d[-1]:
                count+=1 
            if len(d)>2 and d[1]==d[-2]:
                count+=1 
    print(count//2) 
