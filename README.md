Let's learn Nim


### Resources
beginner guides:  
[Nim manual](https://nim-lang.org/docs/manual.html)  
[Nim programming book](https://github.com/StefanSalewski/NimProgrammingBook/blob/master/nimprogramming.adoc)  
[Nim basics](https://narimiran.github.io/nim-basics/)

intermediate guides:  
[Nim tutorial](https://nim-lang.org/docs/tut1.html)  
[Nim by example](https://nim-by-example.github.io)  
[Learn Nim in 5 minutes](https://learnxinyminutes.com/docs/nim/)

sandbox:  
https://play.nim-lang.org/

### Comments
```nim
# comment
## documentation comment
#[ multi-line 
   comment ]#
```

---

### Operators
```nim
+ # addition += # increment = assignment
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
# (re)initializes a variable to a constant
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

### If statement
```nim
if statement:
  expression
elif statement:
  expression
else:
  expression
```

---

### When statement
same as if, except conditions must be constants and statement remains in the same scope. also, code only get generated for the true condition by the compiler
```nim
when statement:
  expression
elif sameStatement:
  expression
else:
  expression
```

### Case statement
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

### For loop
```nim
for i in 1 .. 10:
  expression
```

---

### While loop
```nim
while age == "":
  expression
```

---

### Procedures
```nim
proc onOff(reply: string): bool =
  echo reply, " [0/1]"
  if reply == 0:
    return true
  else:
    return false
    
onOff(0) # true
```

#### Common procedures

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

### Store input
```nim
var line = readLine(stdin)
