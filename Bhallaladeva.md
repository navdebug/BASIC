# BASIC
CodeChef Programs at beginner and easy level
n=int(input())
arr=list(map(int,input().split()))
m=0
sub=[]
q=int(input())
for i in range(q):
    k=int(input())
    if k==0:
        print(sum(arr))
    else:
        for i in range(k):
            a=min(arr)
    
            sub.append(a)
            arr.remove(a)
    
    #sub.append(a)
        print(sum(sub))

            
           
                
        
