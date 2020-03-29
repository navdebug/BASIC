# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    N = int(input())
    array = list(map(int, input().split()))
    result = array[0]
    for i in range(1,N):
        if array[i] > array[i-1]:
            result += (array[i] - array[i-1])
    print(result)
