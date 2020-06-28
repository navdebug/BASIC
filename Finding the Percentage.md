# BASIC
HackerRank Programs at beginner and easy level
INPUT
2
Ashwini 25 26.5 30
Navya 26 27 30
Ashwini

OUTPUT
26.5

if __name__ == '__main__':
    n = int(input())
    l=[]
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores 
    query_name = input()
    l=student_marks[query_name]
    e=sum(l)/3
    print("{:.2f}".format(e))
