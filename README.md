<div align=center>
<a href="https://www.hackerrank.com/priyanshu_706811"><img src="https://github.com/Psingh12354/Java-HackeRank/blob/master/hack.png" width="35%"></img></a>
</div>

<div float=left align=center>
  <img src="https://github.com/Psingh12354/Certificates/blob/master/sql.JPG" width="25%" />
  <img src="https://github.com/Psingh12354/Certificates/blob/master/HackerRank%20Problem%20Solving%20(Basic)).PNG" width="25%" /> 
  <img src="https://github.com/Psingh12354/Certificates/blob/master/C%2B%2B.PNG" width="25%" />
</div>
<div float=left align=center>
  <img src="https://github.com/Psingh12354/Certificates/blob/master/badges.JPG" width="80%" />
</div>

### Python average function

```
import math
import os
import random
import re
import sys



def avg(*nums):
    return sum(nums)/len(nums)

if __name__ == '__main__':
```

### Python Reverse Word and Swap Cases

```
#!/bin/python

import math
import os
import random
import re
import sys



#
# Complete the 'reverse_words_order_and_swap_cases' function below.
#
# The function is expected to return a STRING.
# The function accepts STRING sentence as parameter.
#

def reverse_words_order_and_swap_cases(sentence):
    word_list = sentence.split()
    reversed_list = word_list[:: -1]
    reversed_sentence = " ".join(reversed_list)
    return reversed_sentence.swapcase()


if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    sentence = raw_input()

    result = reverse_words_order_and_swap_cases(sentence)

    fptr.write(result + '\n')

    fptr.close()
```
   
### Python Shape Classes with Area Method 
   
```
#!/bin/python3

import math
import os
import random
import re
import sys



class Rectangle:
    def __init__(self,breadth,length):
        self.breadth=breadth
        self.length=length
    def area(self):
        return self.breadth*self.length

    pass

class Circle:
    def __init__(self,radius):
        self.radius=radius
    def area(self):
        return math.pi*(self.radius**2)
    pass
if __name__ == '__main__':  
```

## Problem Solving 

### Gaming laptop battery life

```
def getBattery(events):
    c=50
    for i in events:
        if (i<0):
            c+=i
        else:
            c+=i
            if c>100:
                c=100
        print(c)
    return c
```

### String Anagram

```
from collections import Counter
def stringAnagram(dictionary, query):
    # Write your code here
    dict = ["".join(sorted(word)) for word in dictionary]
    q = ["".join(sorted(word)) for word in query]
    result = []
    count = Counter(dict)
    for word in q:
        if word in count.keys():
            result.append(count[word])
        else:
            result.append(0)

    return result
```

## Java

### The Adder Class

```
class Adder extends Calculator{
int add(int a,int b)
{
return a+b;
}
}
```

## Sql

### Student Advisor

```
select std.roll_number, std.name 
from student_information std, faculty_information fi 
where std.advisor = fi.employee_id and (fi.gender = 'M' and fi.salary > 15000 or fi.gender = 'F' and fi.salary > 20000) 
```
