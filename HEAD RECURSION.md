# Types of Recursion: Head Recursion in Python

##  AIM:
Write a Python Program to find the sum of all digits in a number using recursion

## ALGORITHM:

1. **Start**
2. Define a recursive function `fun(n)`
3. In the function:
   - Create a recursive call at the **beginning** (Head Recursion)
   - Print the result after the recursive call
4. Take input from the user
5. Call the recursive function
7. **Stop**

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
<img width="338" height="240" alt="image" src="https://github.com/user-attachments/assets/23388787-089e-40ff-83fb-2d8fe281aab0" />

## RESULT
The program was executed successfully
