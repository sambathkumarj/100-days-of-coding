# Given a list of numbers, find and print all its elements that are greater than their left neighbor.

```
Example input
1 5 2 4 3

Example output
5 4
```
list_result=[int(i) for i in input().split()]
j=0
while j<len(list_result):
  if(list_result[j]>list_result[j-1] and j>0):
    print(list_result[j],end="")
  j+=1 
