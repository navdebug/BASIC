# BASIC
CodeChef Programs at beginner and easy level
INPUT 
Hack 2

OUTPUT 
A
C
H
K
AC
AH
AK
CH
CK
HK


from itertools import combinations 
s,n=input().split()
for i in range(1,int(n)+1):
  for j in combinations(s(sorted),int(i)):
      print(''.join(j))
