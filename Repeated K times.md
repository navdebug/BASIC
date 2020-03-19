# BASIC
Hackerearth Programs at beginner and easy level
n=int(input())
arr = list(map(int, input().split()))
k=int(input())
c=0
arr.sort(reverse=False)
a=min(arr)
for j in range(0,n):
    if arr[j]==a:
        c+=1 
if c==k:
    print(a)
            
