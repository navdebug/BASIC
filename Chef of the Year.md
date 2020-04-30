# BASIC
CodeChef Programs at beginner and easy level
import collections
import operator
n,m=map(int,input().split())
a={}
for i in range(n):
    s=input().split()
    a.update({s[0]:s[1]})
#print(a)
ab=[]
for i in range(m):
    ab.append(input())
#print(ab)
l=dict(collections.Counter(ab))
p=list(l.keys())
l=list(l.values())
d=[]
x=max(l)
y=[]
for i in range(len(l)):
    if l[i]==x:
        d.append(p[i])
for i in range(len(ab)):
    y.append(a.get(ab[i]))
x=min(d)
y=dict(collections.Counter(y))
y=sorted(y.items(),key=operator.itemgetter(1))
#print(y)
p=y[len(y)-1][1]
l=[]
for i in range(len(y)):
    if p==y[i][1]:
        l.append(y[i][0])
print(min(l))
print(x)
