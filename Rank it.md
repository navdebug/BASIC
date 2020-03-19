# BASIC
CodeChef Programs at beginner and easy level
n = int(input())
arr1 = list(map(int, input().split()))
q = int(input())
arr2 = []
 
for i in range(0, q):
    arr2.append(int(input()))
 
arr1.sort()
 
def binary_search(bot, top, val):
    while bot <= top:
        mid = int((bot + top)/2)
        if arr1[mid] < val:
            bot = mid
        elif arr1[mid] > val:
            top = mid
        else:
            return mid + 1
 
c = []
for i in range (0, q):
    c.append(binary_search(0, n, arr2[i]))
 
for pos in c:
    print(pos)
