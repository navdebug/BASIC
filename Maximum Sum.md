# BASIC
Hackerearth Programs at beginner and easy level
N = int(input())
num2 = list(map(int,input().split()))
num2.sort(reverse = True)
maximum = num2[0]
maxlist = []
maxlist.append(num2[0])
for i in range(1,N):
    if maximum+num2[i]>=maximum:
        maximum+=num2[i]
        maxlist.append(num2[i])
print(maximum,len(maxlist))
 
