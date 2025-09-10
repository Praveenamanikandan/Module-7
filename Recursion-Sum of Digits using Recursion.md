# #  Recursion:Sum of Digits using Recursion in Python

##  AIM:
To write a Python program to calculate the **sum of all digits** in a number using **recursion**.

##  ALGORITHM:

1. **Start**
2. Define a recursive function `sum_digit(n)` that:
   - Returns 0 if `n <= 0` (Base Case)
   - Else, returns `n % 10 + sum_digit(n // 10)` (Recursive Case)
3. Take integer input from the user.
4. Call the recursive function and store the result.
5. Print the result.
6. **Stop**

## PROGRAM:

```
def sum_of_digits(n):
    if n == 0:
        return 0
    else:
        return (n % 10) + sum_of_digits(n // 10)

# Get input from user
num = int(input())

# Call the recursive function
result = sum_of_digits(num)

# Display result
print(result)

```

## OUTPUT
<img width="402" height="245" alt="image" src="https://github.com/user-attachments/assets/6d0cba04-7865-4dc3-9b4f-51f9577a106a" />

## RESULT
The program was executed successfully
