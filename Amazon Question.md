# BASIC
CodeChef Programs at beginner and easy level
n=int(input())

c=0

ele=(bin(n)[2::1])
a=[int(x) for x in ele]
for i in range(len(a)):
    if a[i]==1:
        c=c+1 
print(c)

    

    
        
