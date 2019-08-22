# Write a program that receives a number on the input.
It also should receive another value 'rev'  (either 0 or 1) on the input. 
If the number is a multiple of 3, or it contains digit 3, it prints "Jugs". 
If the number is a multiple of 5, or it contains digit 5, it prints "Mugs".
If the number is a multiple of 7, or it contains digit 7, it prints "Pugs".

If the number is a multiple of both 3 and 5, it prints "JugsMugs".
      also if number contains 3 and 5, it prints "JugsMugs"
 If the number is a multiple of both 3 and 7, it prints "JugsPugs".
      also if number contains 3 and 7, it prints "JugsPugs"
 If the number is a multiple of 3, 5 and 7, it prints "JugsMugPugs".
      also if number contains 3, 5 and 7, it prints "JugsMugsPugs"

Otherwise, it prints the number.

```
INPUT 
73 
False  # contains 3 and 7

OUTPUT
JugsPugs
```
```
INPUT 
73 
True  # contains 7 and 3, print reverse order

OUTPUT
PugsJugs
```
```
INPUT 
51  # multiple of 3 and contains 5

OUTPUT
JugsMugs
```
```
INPUT 
105

OUTPUT 
JugsMugsPugs

```

num=int(input())
rev=int(input())
if rev==1:
  if (num%3==0 and num%5==0 and num%7==0)or(('3'and'7'and'5') in str(num)):
    print("PugsMugsJugs")
  elif (num%3==0 and num%5==0)or(('3'and'5') in str(num)):
    print("MugsJugs")
  elif (num%3==0 and num%7==0)or(('3'and'7') in str(num)):
    print("PugsJugs")
  elif (num%5==0 and num%7==0)or(('5'and'7') in str(num)):
    print("PugsJugs")
  elif (num%3==0)or('3' in str(num)):
    print("Jugs")
  elif (num%5==0)or('5' in str(num)):
    print("Mugs")
  elif (num%7==0)or('7' in str(num)):
    print("Pugs")
  else:
    print(num)
else:
  if (num%3==0 and num%5==0 and num%7==0)or(('3'and'5'and'7') in str(num)):
   print("JugsMugsPugs")
  elif (num%3==0 and num%5==0)or('3'and'5' in str(num)):
    print("JugsMugs")
  elif (num%3==0 and num%7==0)or('3'and'7' in str(num)):
    print("JugsPugs")
  elif (num%5==0 and num%7==0)or('5'and'7' in str(num)):
    print("MugsPugs")
  elif (num%3==0)or('3' in str(num)):
    print("Jugs")
  elif (num%5==0)or('5' in str(num)):
    print("Mugs")
  elif (num%7==0)or('7' in str(num)):
    print("Pugs")
  else:
    print(num)
