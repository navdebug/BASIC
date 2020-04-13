# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
  n=int(input())
  a=list(map(int,input().split()))
  a.sort()
  m=0
  c=1
  for i in range(n-1):
    if(a[i]==a[i+1]):
      c+=1
    else:
      m=max(m,c)
      c=1
  print(m,c)
  m=max(m,c)
  print(max(m,(n+1)//2))


