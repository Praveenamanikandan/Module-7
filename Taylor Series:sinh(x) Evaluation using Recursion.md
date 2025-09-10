#  Taylor Series:sinh(x) Evaluation using Recursion in Python

##  AIM:
To write a Python program to evaluate the value of **cosh(x)** for **n terms** using recursion.

---

##  ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `cosh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + cosh(x, n - 1)`
6. Call the `cosh(x, n)` function and print the result
7. **Stop**

---

##  PROGRAM:

```
def fact(i):
   if i==1 or i==0:
       return 1
   else:
       return i*fact(i-1)
def cosh(x,n):
  if n==0:
    return 1
  else:
    return(((pow(x,(2*n)))/(fact(2*n))) + cosh(x,n-1))
x=int(input())
n=int(input())
print(cosh(x,n))
```

## OUTPUT
<img width="582" height="240" alt="image" src="https://github.com/user-attachments/assets/986593d2-db8e-4f70-9fbf-415c34b25adc" />

## RESULT
The program was executed successfully
