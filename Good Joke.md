# BASIC
CodeChef Programs at beginner and easy level
for t in range(int(input())):
  ans = 0
  for i in range(int(input())):
    a, b = map(int,input().split())
    ans ^=(i+1)
  print(ans)
