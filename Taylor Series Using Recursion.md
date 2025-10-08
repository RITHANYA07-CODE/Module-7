# 📐 Taylor Series Using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate a **Taylor Series** using **recursion**, where values of `x` and `n` are taken from the user.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `taylor_series(x, n)`
3. In the function:

   * If `n` is 0, return 1 (Base Case)
   * Otherwise, return `taylor_series(x, n-1) + (x^n) / n`
4. Take input `x` from the user
5. Take input `y` from the user
6. Call the function: `result = taylor_series(x, y)`
7. Print `result`
8. **Stop**


## 💻 PROGRAM:

```
def taylor_series(x, n):
    if n == 0:
        return 1 # base class
    return taylor_series(x, n - 1) + (x**n) / n
    
x = int(input())
y = int(input())

result = taylor_series(x, y)
print(result)
```

## OUTPUT
<img width="737" height="234" alt="image" src="https://github.com/user-attachments/assets/a611fb4e-8a6f-4d12-ae87-d66fc53f448a" />


## RESULT
The program successfully evaluates the Taylor Series for the given value of x up to n terms using recursion, and displays the correct sum.
