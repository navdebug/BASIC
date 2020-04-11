# BASIC
CodeChef Programs at beginner and easy level
def solve(l,r,g):
	ans = r//g - l//g
	if l%g==0:
		ans+=1
	if ans == 1:
		if g >= l and g<=r:
			print(ans)
		else:
			print(0)
	else:
		print(ans)

for t  in range(int(input())):
	l, r, g = list(map(int, input().split()))
	solve(l,r,g)
