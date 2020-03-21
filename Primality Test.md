# BASIC
CodeChef Programs at beginner and easy level
from math import sqrt
def IsPrime(n):
    if n==1:
        return False
    for i in range(2,int(sqrt(n))+1):
        if n%i==0:
            return False
    else:
        return True


for _ in range(int(input())):
    if IsPrime(int(input())):
        print('yes')
    else:
        print('no')
