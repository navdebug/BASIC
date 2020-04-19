# BASIC
CodeChef Programs at beginner and easy level
def solve():
	a = list(map(int, input().split()))
	n = a[0]
	k = a[1]
	if n % (k * k) == 0:
		print("NO")
	else:
		print("YES")

t = int(input())
for tt in range(0, t):
	solve()
