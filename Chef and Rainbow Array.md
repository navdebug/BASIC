# BASIC
CodeChef Programs at beginner and easy level
def func(l):
    index = 0
    for i in range(1,8):
        if i not in l:
            return "no"

    ptr1 = 0
    ptr2 = len(l)-1
    while ptr1 <= ptr2:
        if l[ptr1] != l[ptr2]:
            return "no"
        ptr1 += 1
        ptr2 -= 1
    return "yes"

t=int(input())
for _ in range(t):
    n=int(input())
    l=list(map(int,input().split()))
    print(func(l))
