# Given a list of numbers, find and print the elements that appear in it only once. Such elements should be printed in the order in which they occur in the original list.

```
Example input
4 3 5 2 5 1 3 5

Example output
4 2 1
```

x = [int(s) for s in input().split()]
for i in range(len(x)):
  for j in range(len(x)):
    if i != j and x[i] == x[j]:
        break
  else:
    print(x[i], end=' ')
