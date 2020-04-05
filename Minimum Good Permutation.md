# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    N = int(input())
    array = []
    if N % 2 == 0:
        for i in range(0,N//2):
            array.append(2*i + 2)
            array.append(2*i + 1)
    else:
        for i in range(0,N//2):
            array.append(2*i + 2)
            array.append(2*i + 1)
        array.pop(-1)
        array.append(N)
        array.append(N-2)
    print(* array)
