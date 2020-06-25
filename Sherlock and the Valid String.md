# BASIC
Hackerrank Programs at beginner and easy level
#!/bin/python3

import math
import os
import random
import re
import sys
from collections import Counter 

# Complete the isValid function below.
def isValid(s): 
    count2=0 

    res=Counter(s)
    l=list(res.values()) 
    for i in range(len(l)):
        if l[i]==2:
            count2=count2+1
        if count2>2:
            result="NO"
        else:
            result="YES"
    return result

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    result = isValid(s)

    fptr.write(result + '\n')

    fptr.close()
