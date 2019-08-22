# Given a list of numbers, swap adjacent elements in each pair (swap A[0] with A[1], A[2] with A[3], etc.). Print the resulting list. If a list has an odd number of elements, leave the last element intact.

```
Example input
1 2 3 4 5

Example output
2 1 4 3 5
```

list_result = [int(i) for i in input().split()]
for j in range(0,len(list_result),2):
  pop_val=list_result.pop(j)
  list_result.insert(j+1,pop_val)
print(list_result)  
