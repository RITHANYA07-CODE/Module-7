# 📐 Taylor Series:sinh(x) Evaluation using Recursion in Python

## 🎯 AIM:
To write a Python program to evaluate the value of **sinh(x)** for **n terms** using recursion.

---

## 🧠 ALGORITHM:

1. **Start**
2. Read input for variable `x` (angle or number)
3. Read input for variable `n` (number of terms)
4. Define a function `fact(n)`:
   - If `n <= 1`, return 1
   - Else, return `n * fact(n - 1)` (recursive factorial)
5. Define a function `sinh(x, n)`:
   - If `n == 0`, return `x`
   - Else, return `(pow(x, 2*n + 1) / fact(2*n + 1)) + sinh(x, n - 1)`
6. Call the `sinh(x, n)` function and print the result
7. **Stop**

---

## 💻 PROGRAM:

```
def fact(i):
    if i == 0 or i == 1:
        return 1
    else:
        return i * fact(i - 1)

def sinh(x, n):
    if n == 0:
        return x
    else:
        return (x ** (2 * n + 1) / fact(2 * n + 1)) + sinh(x, n - 1)

x = float(input("Enter x: "))
n = int(input("Enter number of terms: "))
print("sinh({}) ≈ {}".format(x, sinh(x, n)))
```

## OUTPUT
<img width="620" height="243" alt="image" src="https://github.com/user-attachments/assets/b72ff5ce-326d-4864-b73b-17b1f9816910" />

## RESULT
The value of sinh(x) has been successfully evaluated using recursion for the given number of terms n in the Taylor series. 
