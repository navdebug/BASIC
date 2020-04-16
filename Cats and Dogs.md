# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    c,d,l=map(int,input().split())
    if l >= max((c - d),(d - c))*4 and l <= (c + d)*4 and l % 4 == 0 and l > 4*d - 1:
        print('yes')
    else:
        print('no')
