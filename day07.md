## Given two timestamps of the same day: a number of hours, minutes and seconds for both of the timestamps. The moment of the first timestamp happened before the moment of the second one. Calculate how many seconds passed between them.

```
Example input #1
1
1
1
2
2
2

Example output #1
3661

Example input #2
1
2
30
1
3
20

Example output #2
50

```
hour1 = int(input())
mintue1 = int(input())
second1 = int(input())
hour2 = int(input())
mintue2 = int(input())
second2 = int(input())
result1 = ((mintue1 * 60) + (hour1 * 3600) + second1)
result2 = ((mintue2 * 60) + (hour2 * 3600) + second2)
print(result2 - result1)
