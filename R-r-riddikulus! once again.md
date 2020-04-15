# BASIC
Hackerearth Programs at beginner and easy level
import collections
t=int(input())
for i in range(t):
    n,k=map(int,input().split())
    arr=list(map(int,input().split()))
    e=collections.deque(arr)
    e.rotate(-k)
    for i in e:
        print(i,"",end="")
