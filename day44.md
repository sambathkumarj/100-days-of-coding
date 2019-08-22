# The text is given in a single line. For each word of the text count the number of its occurrences before it.

```
Example input
one two one two three two four three

Example output
0 0 1 1 0 2 0 1

```
def occ(s):
   flag = {}
   string = ''
   for word in s.split():
      flag[word] = flag.get(word, 0) + 1
      string += str(flag[word] - 1) +' '
   return string

print(occ(input()))
