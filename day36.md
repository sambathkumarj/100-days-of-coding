# Given a list of numbers, find and print all its elements with even indices (i.e. A[0], A[2], A[4], ...).

```
Example input
5 6 7 8 9

Example output
5 7 9
```

list_num=[int(i) for i in input().split()]
print(list_num[0: :2])
