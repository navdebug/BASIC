# BASIC
CodeChef Programs at beginner and easy level
from math import sqrt
a,b,c=int(input()),int(input()),int(input())
if((b**2 - (4*a*c)) == 0):
    print(-b/(2*a),-b/(2*a),sep="\n")
else:
    n=(b**2)-(4*a*c)
    print((-b+sqrt(n))/(2*a),(-b-sqrt(n))/(2*a) ,sep="\n")
