# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
lst=[]
sub=[]
c=0
for _ in range(t):
    n=int(input())
    arr=list(map(int,input().split()))
    for i in arr:
        if i%4!=0:
            arr.remove(i)
            lst.append(i)
        
    #print(arr,lst)
    for j in range(0,len(lst)):
        for k in range(j,len(lst)):
            if (lst[j]+lst[k])%4==0:
                arr.append(lst[j]+lst[k])
                c=c+1
    #print(arr)            
    print(c+1)
            
            
    
