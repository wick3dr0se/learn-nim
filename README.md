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

<h2 align="center">Comments</h2>

```nim
# comment
## documentation comment
#[ multi-line 
   comment ]#
```

<h2 align="center">Operators</h2>

### Arithmetic Operators
calculate numerical values
```nim
+ # add
- # subtract
* # multiply
/ # divide
^ # power
```

### Assignment Operators
define a value
```nim
= # assign
+= # add, assign
```

### Logical Operators
test if conditions are true or not
```nim
# following operators return true, if:
and # both conditions are true
or # condition(s) is true
xor # a condition is true and other is not
not # condition is false (accepts a single condition)
```

### Relational operators
test the relation between two comparable conditions
```nim
== # is equal   != # not equal
> # greater than   >= greater or equal
< # lesser than   <= less or equal
```

<h2 align="center">Data Types</h2>

### Data types
declares how values are interpreted
```nim
bool # true/false
int # integer
float # floating-point number
char # a single character (single quotes)
string # character array (double quotes)
```

<h2 align="center">Variables</h2>

### var
define (& declare) a data type of mutable value
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

### const
define a constant of immutable value
```nim
# define constant
const Pi = 3.14
  
# define constant block
const
  Pi = 3.14
  four = 4
  apple = red
```

### let
declares & defines a(n existing) variable to an immutable value
```nim
let n = 2
```

<h2 align="center">Types</h2>

### array
a collection of strings
```nim
type
  TwoArgs = array[2, strings]
```

### enum
a group of constants
```nim
type
  Signals = enum
    sigQuit = 3, sigAbort = 6, sigKill = 9
```

<h2 align="center">Statements</h2>

### if
branch control flow, good for 3/4 expressions
```nim
if Pi == 3.14:
  echo "Let's have Pi"
elif apple == red:
  echo "Apples are red"
else:
  echo "Neither apples are read nor Pi equal 3.14"
```

### when
same as if, except with constants and statement remains in the same scope
```nim
when apple == red:
  return true
elif apple == orange:
  return false
```

### case
multi-branch control flow, good for more than 3 expressions
```nim
case "Pi":
  of "blueberey":
    "fail"
  of "3.14":
    "pass"
  else:
    "impossible"
```

_control flow statements will be executed only if some condition is satisfied_

<h2 align="center">Loops</h2>

### for
iterate until condition is met
```nim
for i in 1 .. 10:
  echo i
```

### while
execute until condition is false
```nim
while true:
  echo "This will never stop"
```

<h2 align="center">Procedures</h2>

### proc
```nim
proc onOff(reply: char): bool =
  echo reply, " [y/n]"
  if reply == y:
    return true
  else:
    return false
    
onOff(y) # true
```
