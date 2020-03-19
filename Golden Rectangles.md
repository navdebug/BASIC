# BASIC
CodeChef Programs at beginner and easy level
from sys import stdin, stdout
res=0
for _ in range(int(stdin.readline())):
    w,h=map(int,stdin.readline().split())
    w=w/1000000000
    h=h/1000000000
    r=w/h
    s=h/w 
#print(r,s)
        if r>=1.6 and r<=1.7:
            res+=1
        if s>=1.6 and s<=1.7:
            res+=1
    stdout.write(str(res))
