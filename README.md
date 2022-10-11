Let's learn Nim


### Resources
beginner guides:  
[Nim programming book](https://github.com/StefanSalewski/NimProgrammingBook/blob/master/nimprogramming.adoc)

intermediate guides:  
[Nim tutorial](https://nim-lang.org/docs/tut1.html)  
https://nim-by-example.github.io/

sandbox:  
https://play.nim-lang.org/

### Comments
```nim
# comment

#[ multi-line 
   comment ]#
```

---

### Operators
```nim
+ # addition += # increment
- # subtraction
* # multiplication
/ # division
^ # power
```

---

### Test operators
```nim
== # is equal to
```
---

### Data types
```nim
bool # true/false
int # integer
float # floating-point number
string # character array
```

---

### Subrange types
```nim
age = 20 .. 30 # implicit range[] keyword
```

---

### Variables
```nim
# declare variable
var n: int

# define variable
n = 1

# declare & define variable
var n: int = 1

# multi-variable declaration
var
  n, i: int
  
# declare & define multi-variable
var n, i: int = 1

# declare variable block
var
  n: int
  name: char
```

---

### Constants
```nim
# define constant
const Pi = 3.14
  
# define constant block
const
  Pi = 3.14
  Four = 2 + 2
```

---

### Let
```nim
# let can be used to reinitialize a variable to a constant value or to store command output
let n = 2
```

---

### Enums
```nim
type
  Signals = enum
    sigQuit = 3, sigAbort = 6, sigKill = 9
```

---

### Arrays
```nim
type
  TwoArgs = array[2, strings]
```

---

### Common procedures
```nim
echo() # output to stream w/ newline
write() # output to stream
inc() # increment by 1 or specification
```

---

### Common functions
```nim
readLine() # read a line
```

---

### Read input
```nim
var line = readLine(stdin)
```

---

### Test
```nim
n == i # equality
```

---

### If-else
```nim
if n == i:
  expression
elif n == Pi:
  expression
else:
  expression
```

---

### Case
```nim
case "Pi":
  of "blueberey":
    "fail"
  of "3.14":
    "pass"
  else:
    "impossible"
```

---

### Loops
```nim
for i in 1 .. 10:
  expression
```
