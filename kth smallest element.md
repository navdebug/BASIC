lst=[]
t=int(input())
for i in range(0,t):
    s=int(input())
    for j in range(0,s):
        ele=int(input())
        lst.append(ele)
    k=int(input())
    lst.sort()
    print(lst[k-1])
        
   
    
    
