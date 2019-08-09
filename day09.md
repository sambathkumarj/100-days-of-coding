## Given a three-digit number. Find the sum of its digits.

```
Example input
123

Example output
6
```
# Read an integer:
a = int(input())
# Print a value:
sum=0
while(a>0):
    result=a%10
    sum=sum+result
    a=a//10
print(sum)
# print(a)
