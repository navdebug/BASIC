# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
	a,b=list(map(int,input().split()))
	if((a%b==0 or b%a==0)):
		print("NO")
	elif(a==b):
		print("NO")
	else:
		print("YES")
