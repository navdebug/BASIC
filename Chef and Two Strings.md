# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
while(t>0):
    s1=input()
    s2=input()
    l=0
    h=0
    n=len(s1)
    for i in range(0,n):
        if(s1[i]!='?' and s2[i]!='?' and s1[i]!=s2[i]):
            l+=1
            
        if(s1[i]=='?' or s2[i]=='?' or s1[i]!=s2[i]):
            h+=1
            #print(s1[i],s2[i])
        
    print(l,h)
    
    t-=1
