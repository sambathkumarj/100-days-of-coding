# Given a list of distinct numbers, swap the minimum and the maximum and print the resulting list.

```
Example input
3 4 5 2 1

Example output
3 4 1 2 5

```

list_result= [int(i) for i in input().split()]
minimum=list_result.index(min(list_result))
maximum=list_result.index(max(list_result))
list_result[minimum],list_result[maximum]=list_result[maximum],list_result[minimum]
print(list_result)

