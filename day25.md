# For given integer n ≤ 9 print a ladder of n steps. The k-th step consists of the integers from 1 to k without spaces between them.

To do that, you can use the sep and end arguments for the function print().

```
Example input
3

Example output
1
12
123
```

result=int(input())
if result<=9:
  x=""
  for s in range(1,result+1):
    s=str(s)
    x=x+s
    print(x)
