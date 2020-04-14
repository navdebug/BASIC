# BASIC
CodeChef Programs at beginner and easy level
def hey(a,x,y):
    c=0
    for k in range(x):
        for j in range(k+1,x):
            if((a[k]+a[j])==y):
              c+=1
              return 1
              break
        if(c>1):
            break
t=int(input())
for i in range(t):
    x,y=map(int,input().split())
    a=[int(x)for x in input().split()]
    b=hey(a,x,y)
    if(b==1):
       print('Yes')
    else:
        print('No')
