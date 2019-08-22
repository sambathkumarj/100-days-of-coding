# Given a sequence of distinct non-negative integers, where each number is written in a separate line. The sequence ends with 0. Print the second largest element in this sequence. It is guaranteed that the sequence has at least two elements.

```
Example input
1
7
9
0

Example output
7

```

result = int(input())
x = 0
y = 0

while result != 0:
  if result > x:
    y = x
    x = result
  else:
    if y < result:
      y = result
  result = int(input())  
print(y)
