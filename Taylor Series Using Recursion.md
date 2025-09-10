#  Taylor Series Using Recursion in Python

##  AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

##  ALGORITHM:

1. **Start**
2. Create variables `x` and `n`
3. Get values for `x` and `n` from the user
4. Define a recursive function `series(x, n)`
   - **Base case:** If `n == 0`, return 1
   - **Recursive case:** Return `x**n / n + series(x, n-1)`
5. Print the result
6. **Stop**

##  PROGRAM:
```
def power(x, n):
    if n == 0:
        return 1
    else:
        return x * power(x, n - 1)

def series_sum(x, n):
    if n == 0:
        return 1
    else:
        return power(x, n) + series_sum(x, n - 1)

x = int(input())
n = int(input())
result = series_sum(x, n)
print(result)

```

## OUTPUT
<img width="420" height="234" alt="image" src="https://github.com/user-attachments/assets/383b2e68-35f4-4e7d-8a05-e792f3ea00d8" />

## RESULT
The program was executed successfully
