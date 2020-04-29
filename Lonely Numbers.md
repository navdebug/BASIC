# BASIC
CodeChef Programs at beginner and easy level
def my_function(s):
    d=[]
    for i in s:
        d.append(s.count(i)) 
    for j in range(len(d)):
        if d[j]==1:
            print(s[j])
s1=list(map(int,input().split()))
a=list(set(s1)) 
my_function(s1)
