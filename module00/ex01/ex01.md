# Exercise 01 - Rev Alpha

|                         |                    |
| -----------------------:| ------------------ |
|   Turn-in directory:    |  ex01              |
|   Files to turn in:     |  exec.py           |
|   Forbidden functions:  |  None              |
|   Remarks:              |  n/a               |

You will have to make a program that reverses the order of a string and the case of its words.  
If we have more than one argument we have to merge them into a single string and separate each arg by a ' ' (space char).

**Example:**

import sys
string = sys.argv
i=len(sys.argv)-1
reverse = ""
t = 0
while i>= 1:
    t = len(string[i]) -1
    while t >= 0:
        if string[i][t].isupper():
            reverse += (string[i][t]).lower()
        else:
            reverse += (string[i][t]).upper()
        t = t - 1
    i -= 1
print(reverse)

