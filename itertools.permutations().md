# BASIC
CodeChef Programs at beginner and easy level
INPUT
HACK 2

OUTPUT
AC
AH
AK
CA
CH
CK
HA
HC
HK
KA
KC
KH

from itertools import permutations
s,n = input().split()
print(*[''.join(i) for i in permutations(sorted(s),int(n))],sep='\n')
