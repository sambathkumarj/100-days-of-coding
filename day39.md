# Given a list of numbers with all elements sorted in ascending order, determine and print the number of distinct elements in it.

```
Example input
1 2 2 3 3 3

Example output
3
```

result = 1
list_num = [int(i) for i in input().split()]
for j in range(1, len(list_num)):
  if list_num[j - 1] != list_num[j]:
    result+= 1
print(result)
