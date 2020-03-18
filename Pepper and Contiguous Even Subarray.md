# BASIC
Hackerearth Programs at beginner and easy level
t=int(input())
sub=[]
ms=-1
for _ in range(0,t):
  n = int(input())
  arr=[int(i) for i in input().split()]
  for h in range(0,n):
    if(arr[i]%2==0):
      sub.append(arr[i])
     if(len(sub)>ms):
      ms=len(sub)
  print(ms)
  
