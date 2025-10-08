# # 🔁 Recursion:Sum of Digits using Recursion in Python

## 🎯 AIM:
There are N people standing in a queue. Each person is given a number of cakes based on their count in the queue. For example, if the person standing fifth in the queue will be given 5 cakes. Construct a python program to tell the total number of cakes required to  procure as per the size of the queue using tail recursion.

## 🧠 ALGORITHM:

1. **Start**
2. Define a recursive function `total_cakes(n, acc)` where:

   * `n` → number of people remaining in the queue
   * `acc` → accumulator to store the running total of cakes
3. In the function:

   * **Base Case:** If `n == 0`, return `acc` (total cakes)
   * **Recursive Case:** Call `total_cakes(n - 1, acc + n)`

     * Add the current person's cakes (`n`) to `acc`
     * Pass the updated `acc` in the recursive call
4. Take input from the user: `N` → total number of people in the queue
5. Call the function → `total_cakes(N, 0)` and store the result
6. Print the result
7. **Stop**


## 💻 PROGRAM:

```
def total_cakes(n, acc=0):
    # Base Case: if queue is empty
    if n == 0:
        return acc
    # Tail Recursive Call: add current person's cakes to accumulator
    return total_cakes(n - 1, acc + n)

# Input: number of people in the queue
N = int(input("Enter the number of people in the queue: "))

# Function call
result = total_cakes(N)

# Output
print(f"Total number of cakes required: {result}")

```
## OUTPUT

<img width="744" height="281" alt="image" src="https://github.com/user-attachments/assets/a8118b4a-2146-449c-b00b-02289b201bbf" />


## RESULT
The Python program successfully calculates the total number of cakes required for N people in a queue using tail recursion.
