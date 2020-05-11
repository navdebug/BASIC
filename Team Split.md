# BASIC
CodeChef Programs at beginner and easy level
t = int(input())
for _ in range(t):
    str_arr = input().split(' ')
    arr = [int(num) for num in str_arr]
    n,a,b,c,d = arr[0],arr[1],arr[2],arr[3],arr[4]
    s = []
    s.append(d)
    for i in range(0,n-1):
        s.append((a*s[i]*s[i]+b*s[i]+c)%1000000)
    s.sort()
    cnt = 0
    if(n%2==0):
        for i in range(0,n-1,2):
            cnt+=s[i+1]-s[i]
    else:
        for i in range(n-1,1,-2):
            cnt+=s[i]-s[i-1]
        cnt+=s[0]
    print(cnt)

        
