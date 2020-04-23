# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for j in range(t):
    N = int(input())
    L= [int(x) for x in input().split()]
    [A, B, C] = [int(x) for x in input().split()]
    S = input()
    for i in range(N):
        if S[i] == 'R':
            y = L[i:]
            L = L[:i]+y[::-1]
        elif S[i] == 'A':
            L[i:] = [x+A for x in L[i:]]
        elif S[i] == 'M':
            L[i:] = [x*B for x in L[i:]]
        L[i:] = [x%C for x in L[i:]]

        print (L[i] , end =' ')
    print()
