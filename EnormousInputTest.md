(n,k)=map(int,input().split(' '))
count=0
for i in range(n):
    m=int(input())
    if m%k==0:
        count+1;
print(count)
