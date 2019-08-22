# Given a list of numbers, print all its even elements. Use a for-loop that iterates over the list itself and not over its indices. That is, don't use range()

```
Example input
1 2 2 3 3 3 4

Example output
2 2 4
```

list_result=[int(i) for i in input().split()]
for j in list_result:
  if(j%2==0):
    print(j)
