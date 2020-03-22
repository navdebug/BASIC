# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for _ in range(t):
    n,v1,v2=map(int,input().split())
    chef=2**0.5*n/v1
    ele=2*n/v2
    # print(chef,ele)
    if(chef>ele):
        print("Elevator")
    else:
        print("Stairs")
