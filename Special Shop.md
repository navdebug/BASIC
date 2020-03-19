# BASIC
Hackerearth Programs at beginner and easy level
num = int(input()) 
while num > 0:
    num -= 1
    n, q, z = map(int,input().split())
    x = round((z*n)/(q+z))
    y = n - x
    print(((q*(x**2))+(z*(y**2))))
