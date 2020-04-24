# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n = int(input())
    m = list(map(int,input().split()))
    m.sort()
    print((n-1)*m[0])
