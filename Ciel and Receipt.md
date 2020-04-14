# BASIC
CodeChef Programs at beginner and easy level
l=[1,2,4,8,16,32,64,128,256,512,1024,2048]
l.reverse()
for _ in range(int(input())):
    n=int(input())
    cnt=0;
    for i in l:
        if n<=0:
            break;
        if n%i<n:
            x=n//i;
            cnt+=x;
            n=n-i*x;
    print(cnt)
