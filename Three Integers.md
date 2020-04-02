# BASIC
CodeChef Programs at beginner and easy level
t=int(input())

for i in range(t):
	x=list(map(int, input().rstrip().split()))
	a=x[0]
	b=x[1]
	c=x[2]
	d=(b-a)-(c-b)
	if(d==0):
		print(0)
	elif((d%2) == 0):
		print(abs(d//2))
	else:
		print(abs(d)//2+1)
