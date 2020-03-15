    n = int(input())
    if n==2:
        print(0)
    elif n==1:
        print(1)
    else:
        ans=(n-(n//2-n//4)*2)
    print(ans)
