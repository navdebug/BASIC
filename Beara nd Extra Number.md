# BASIC
CodeChef Programs at beginner and easy level
t = int(input())
while t >= 1:
	t -= 1
	n = int(input())
	arr = input()
	arr = arr.split(" ")[:n]
	arr = [int(x) for x in arr]
	arr.sort()
	if abs(arr[0]-arr[1]) == 0 or abs(arr[0]-arr[1]) > 1:
		print(arr[0])
	elif abs(arr[n-2]-arr[n-1]) == 0 or abs(arr[n-2]-arr[n-1]) > 1:
		print(arr[n-1])
	else:
		for i in range(n-1):
			if arr[i] == arr[i+1]:
				print(arr[i])
				break
