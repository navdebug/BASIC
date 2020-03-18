# BASIC
Hackerearth Programs at beginner and easy level
n=int(input())
d=dict()
for _ in range(0,n):
    name,score=tuple(input().split())
    d[name] = int (score)

vals=list(d.values())
keys=list(d.keys())
v=sorted(vals,reverse=True)[:3]
for i in v:
    print(keys[vals.index(i)])
    
