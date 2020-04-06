# BASIC
CodeChef Programs at beginner and easy level
from math import  gcd
t =int(input())


for i in range(t):
    n = int(input())
    l = list(map(int,input().split()))
    z = 0
    for i in range(n):
        z = gcd(z,l[i])
    print(z*n)
