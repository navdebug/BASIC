# BASIC
CodeChef Programs at beginner and easy level
for t in range(int(input())):
    n = int(input())
    land = [int(i) for i in input().split()]
    if n % 2:
        valid = [i for i in range(1, n //2 + 1)]
        valid += [i for i in range(n //2 + 1, 0, -1)]
        if valid == land:
            print("yes")
        else:
            print("no")
    else:
        print("no")
