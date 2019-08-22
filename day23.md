# For the given integer N calculate the following sum:

1³ + 2³ + ... + N³

```
Example input
3

Example output
36
```

result=int(input())
a=[]
for i in range(1,result+1):
  b=i**3
  a.append(b)
print(sum(a))
