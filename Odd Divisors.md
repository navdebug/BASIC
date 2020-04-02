# BASIC
CodeChef Programs at beginner and easy level
def f(n):
    sum = 0
    for i in range(1,n+1,2):
        m = n // i
        sum += (i*m)
    return sum

for i in range(int(input())):
    total = 0
    l, r = map(int, input().split())
    total = f(r) - f(l-1)
    print(total)
