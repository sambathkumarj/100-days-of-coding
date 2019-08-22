# Given a list of non-zero integers, find and print the first adjacent pair of elements that have the same sign. If there is no such pair, print 0.

```
Example input #1
-1 2 3 -1 -2

Example output #1
2 3

Example input #2
1 -3 4 -2 1

Example output #2
0
```

result = input()
x = list(map(int, result.split()))
i = 1

for i in range(1, len(x)):
  if x[i] * x[i-1] > 0:
    print(str(x[i - 1]), str(x[i]))
    break
  elif i == len(x)-1:
    print("0")
