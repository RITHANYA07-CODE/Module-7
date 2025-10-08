# 🔁 Recursion:Palindrome Checker Using Recursion in Python

## 🎯 AIM:
To write a Python program to check whether a given string is a **palindrome** using **recursion**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `is_palindrome(word)`
   - **Base Case:** If the string length is less than 1, return `True`
   - **Recursive Case:** If the first and last characters match, call the function recursively on the substring without first and last characters
   - Else, return `False`
3. Get input from the user
4. Call the recursive function
5. Print whether the string is a palindrome
6. **Stop**

---

## 💻 PROGRAM:
```
def is_palindrome(word):
    
    if len(word) <= 1:
        return True;
    if word[0] != word[-1]:
        return False;
    return is_palindrome(word[1 : -1])
    
input_str = input()

if is_palindrome(input_str):
    print("String is a palindrome");
else:
    print("String is not a palindrome")
```

## OUTPUT
<img width="854" height="334" alt="image" src="https://github.com/user-attachments/assets/af4ff63f-256e-41f0-b539-3fc9fea5c5fb" />


## RESULT
The Python program successfully checks whether a given string is a palindrome using recursion.
