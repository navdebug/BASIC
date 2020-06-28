# BASIC
CodeChef Programs at beginner and easy level
INPUT
HACK 2

OUTPUT
AA
AC
AH
AK
CC
CH
CK
HH
HK
KK

from itertools import combinations_with_replacement
s,n=int(input())
print(*[''.join(i) for i in combinations_with_replacemnt(sorted(s),int(n))],sep='\n']
