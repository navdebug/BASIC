# BASIC
Hackerearth Programs at beginner and easy level
for _ in range(int(input())):
    n, k = map(int, input().split(' '))
    l = min(map(int, input().split(' ')))
    #sm = min(n_list)
    if l < k: print(k - l)
    else: print(0)
