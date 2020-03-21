# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n, k = map(int, input().split())
    words = input().split()
    output = ''
    str= []

    for i in range(k):
        str += input().split()

    for w in words:
        if w in str:
            output = output + 'YES '
        else:
            output = output + 'NO '

    print(output.strip())

