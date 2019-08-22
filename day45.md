# Given the text: the first line contains the number of lines, then given the lines of words. Print the word in the text that occurs most often. If there are many such words, print the one that is less in the alphabetical order.

```
Example input
2
apple orange banana
banana orange

Example output
banana

```
s=int(input())
x={}
list1=[]
for i in range(s):
  a=list(input().split())
  for t in range(len(a)):
    if a[t] not in x:
      x[a[t]]=0
    x[a[t]]+=1
for k,v in x.items():
  if v>=max(x.values()):
    list1.append(k)
print(sorted(list1)[0])
    
