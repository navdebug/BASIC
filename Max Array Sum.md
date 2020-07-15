# BASIC
Hackerank Programs at beginner and easy level

INPUT
5
1 2 3 4 5

OUPUT 
9 

def SumArray(arr):
    dp=[]
    dp.append(arr[0])
    dp.append(max(arr[:2]))
    ans=max(dp)
    for i in arr[2:]:
        dp.append(max(max(dp[-2]+i,i),ans)) 
        ans=max(ans,dp[-1])
    return ans 
n=int(input())
arr=list(map(int,input().split()))

res=SumArray(arr)
print(res)
