# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    n = int(input())
    a = [0]
    a.extend(list(map(int, input().split())))
    dp = [0] * (n + 1)
    dp[1] = a[1]
    for i in range(2, n + 1):
        dp[i] = max(dp[i - 1] + a[i] * i, dp[i - 2] + i * a[i - 1] + (i - 1) * a[i])
    
    print(dp[n])
        
    
        
