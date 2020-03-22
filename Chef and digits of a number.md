# BASIC
CodeChef Programs at beginner and easy level
# cook your dish here
for _ in range(int(input())):
    d = input()
    count_0 = d.count('0')
    count_1 = d.count('1')
    if count_0 == 1 or count_1 ==1:
        print('Yes')
    else:
        print('No')
