# BASIC
CodeChef Programs at beginner and easy level
# cook your dish here
for _ in range(int(input())):
    input()
    lis = list(map(int,input().split()))
    print(sum(lis) - min(lis)*len(lis))
