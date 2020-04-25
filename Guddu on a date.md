# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(t):
    n=int(input())
    st=str(n)
    l=list(st)
    for j in range(len(l)):
        l[j]=int(l[j])
    s=sum(l)
    m=s%10 
    if m!=0:
        m=10-m 
    r=st+str(m)
    print(int(r))
