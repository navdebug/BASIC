# BASIC
CodeChef Programs at beginner and easy level
try:
    for t in range(int(input())):
        # TODO: write code...
        n = int(input())
        arr = input().split()
        start = arr.index('1')
        count =0
        ans='NO'
        if(arr.count('1')<2):
            ans='YES'
        else:
            for i in arr[start+1:]:
                if(i=='0'):
                    count+=1
                if(i=='1'):
                    if(count>=5):
                        ans='YES'
                        count=0
                        continue
                    else:
                        ans='NO'
                        break
        print(ans)
except Exception as e:
    pass
