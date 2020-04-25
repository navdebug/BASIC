# BASIC
CodeChef Programs at beginner and easy level
for _ in range(int(input())):
    a=[]
    n=int(input())
    for i in range(n):
        s=input()
        a.append(s)
    x=""
    x= x.join(a) 
    a1=x.count("c")//2
    a2=x.count("o")
    a3=x.count("d")
    a4=x.count("e")//2
    a5=x.count("h")
    a6=x.count("f")
    l=[a1,a2,a3,a4,a5,a6]
    print(min(l))
