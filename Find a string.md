# BASIC
Hackerank Programs at beginner and easy level
INPUT

ABCDCDC
CDC

OUPUT
2

def count_substring(string, sub_string):
    count=0
    ls=len(string)
    ls1=len(sub_string)
    for i in range(ls):
        if string[i:i+ls1]==sub_string:
            count=count+1 
    return count
