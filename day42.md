# It is possible to place 8 queens on an 8×8 chessboard so that no two queens threaten each other. Thus, it requires that no two queens share the same row, column, or diagonal.  

Given a placement of 8 queens on the chessboard. If there is a pair of queens that violates this rule, print YES, otherwise print NO. The input consists of eight coordinate pairs, one pair per line, with each pair giving the position of a queen on a standard chessboard with rows and columns numbered from 1 to 8.

```
Example input
1 5
2 3
3 1
4 7
5 2
6 8
7 6
8 4
(shown on the picture)

Example output
NO
```

x=[]
y=[]
result=8
for i in range(result):
  a,b = [int(s) for s in input().split()]
  x.append(int(a))
  y.append(int(b))

res=1
for i in range(result):
  for j in range(i+1,result):
    if(x[i]==x[j] or y[i]==y[j] or abs(x[i]-x[j])==abs(y[i]-y[j])):
      res=0
if res:    
  print("No")
else:
  print("Yes")
