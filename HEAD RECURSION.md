# 🔁 Types of Recursion: Head Recursion in Python

## 🎯 AIM:
Write a Python program to display Arithmetic Progression  series by reading the difference between the numbers and limit  using  head recursion.

## 🧠 ALGORITHM:

1. Define a recursive function `fun(n, d)`
2. In the function:

   * Check if `n > 0`
   * If **True**:

     1. Make a **recursive call** → `fun(n - d, d)`  *(Head Recursion)*
     2. After the recursive call returns, **print** the value of `n`
3. Read two inputs from the user:

   * `d` → common difference between terms
   * `x` → last term (limit) of the series
4. Call the function → `fun(x, d)`


## 💻 PROGRAM:

```
def fun(n,d):
    if (n > 0):
        fun(n - d,d)
        print(n, end=" ")
 
d= int(input())
x = int(input())
fun(x,d)

```

## OUTPUT
<img width="1261" height="251" alt="image" src="https://github.com/user-attachments/assets/ba4af7bc-1d00-480a-ba3a-6f560aa4ceda" />


## RESULT
The program successfully displays the Arithmetic Progression (A.P.) series using Head Recursion.
