# BASIC
CodeChef Programs at beginner and easy level
t = int(input())
while t:
    n = int(input())
    A = list(map(int, input().split()))
    A.sort()
    count = 1
    m = 0
    for i in range(n-1):
        if A[i]==A[i+1]:
            count += 1
        else:
            m = max(m,count)
            count = 1
    m = max(m,count)
    print(n-m)
    t -= 1
