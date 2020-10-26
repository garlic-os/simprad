# simprad
_Simplify radicals._

Simplifies a radical into a multiple of the square root of a prime number.
Based on the popular SIMPRAD for TI-BASIC of unknown author.
Supports negative numbers and arbitrary roots.

When the input is a nonnegative number, the output will be a Tuple of two
real numbers&#2014;the coefficient and the radicand.  
When the input is a negative number, the output will be a Tuple of a complex
coefficient and a real radicand.

Use simprad as a module:
```py
from simprad import simprad

print(simprad(50))    # (5, 2)
print(simprad(36))    # (6, 1)
print(simprad(-50))   # (5j, 2)
print(simprad(8, 3))  # (2, 1)
```

Use simprad as a command line utility:
```sh
$ python -m simprad
Radical to simplify: &#221A;50
Root [2]: 2
5 &#00D7; &#221A;2
```
