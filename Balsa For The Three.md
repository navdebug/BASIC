# BASIC
CodeChef Programs at beginner and easy level
t=int(input())
for i in range(0,t):
    g=int(input())
    g+=1 
    while str(g).count("3")<3:
        g=g+1 
    print(g)
