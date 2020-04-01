# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    S = input()
    a = b = 0
    for i in range(len(S)):
        a += 1 if ((S[i] == '-' and i % 2 == 0) or 
                    (S[i] == '+' and i % 2 == 1)) else 0
        b += 1 if ((S[i] == '-' and i % 2 == 1) or
                    (S[i] == '+' and i % 2 == 0)) else 0
    print(min(a, b))
