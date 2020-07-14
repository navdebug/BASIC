# BASIC
Hackerank Programs at beginner and easy level

INPUT 
aabbcd 

OUTPUT 
NO 

from collections import Counter
def isValid(S):
    char_map = Counter(S)
    char_occurence_map = Counter(char_map.values())
 
    if len(char_occurence_map) == 1:
        return True
 
    if len(char_occurence_map) == 2:
        for v in char_occurence_map.values():
            if v == 1:
                return True
 
    return False
 
 
S = raw_input()
if isValid(S):
    print "YES"
else:
    print "NO"
