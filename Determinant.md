# BASIC
CodeChef Programs at beginner and easy level
import numpy as np
n=int(input())
arr=list(map(int,input().split()))
matrix =np.array(arr).reshape(n,n)
print(np.linalg.det(matrix))
