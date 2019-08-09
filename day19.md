## Write a program that receives a number on the input.

  - If the number is a multiple of 3, or it contains digit 3, it prints "Jugs". 
  - If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".
  - If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".

Otherwise, it prints the number.
```

INPUT 
73 
OUTPUT
JugsPugs

INPUT 
51  

OUTPUT
JugsMugs


INPUT 
105

OUTPUT 
JugsMugsPugs

```
result=int(input())
if(result%3==0 or '3' in str(result)):
  print("Jugs")
if(result%5==0 or '5' in str(result)):
  print("Mugs")
if(result%7==0 or '7' in str(result)):
  print("Pugs")

