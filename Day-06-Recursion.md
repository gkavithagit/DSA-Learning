📌 Day 6 — Recursion

📖 What I Learned

Today I learned the fundamentals of Recursion, an important problem-solving concept in Data Structures and Algorithms.

Recursion is a technique where a function calls itself to solve a smaller version of the same problem.

🔹 Basic Structure of Recursion

A recursive solution generally contains two important parts:

1. Base Case — The condition that stops the recursion.
2. Recursive Case — The part where the function calls itself with a smaller or simpler input.

def countdown(n):
    if n == 0:
        return

    print(n)
    countdown(n - 1)

🔹 How Recursion Works

For:

countdown(3)

The calls happen like this:

countdown(3)
     ↓
countdown(2)
     ↓
countdown(1)
     ↓
countdown(0)
     ↓
   STOP

The function calls are stored in the call stack until the base case is reached.

🧠 Key Concepts

- Recursion
- Base Case
- Recursive Case
- Function Calls
- Call Stack
- Stack Unwinding
- Recursion vs Iteration
- Time and Space Complexity of recursive solutions

📦 Call Stack

Each recursive function call requires a stack frame.

Conceptually:

┌──────────────┐
│ countdown(1) │
├──────────────┤
│ countdown(2) │
├──────────────┤
│ countdown(3) │
└──────────────┘

Once the base case is reached, the stack begins to unwind.

🔄 Recursion vs Loop

A loop can often solve the same problem more simply, but recursion becomes especially useful for problems involving:

- Trees
- Graphs
- DFS
- Backtracking
- Divide and Conquer
- Dynamic Programming

💻 Practice

Problem: Print numbers from 1 to N

Example:

Input: 5
Output: 1 2 3 4 5

I practiced identifying:

- The base case
- The recursive case
- How the function moves toward the base case
- How recursive calls are stored in the call stack

🎯 Key Takeaway

The most important lesson from today:

«Every recursive solution needs a clear stopping condition and a recursive step that moves toward that stopping condition.»

Understanding the call stack is essential for analyzing the space complexity of recursive algorithms.

---

📈 DSA Progress

Day| Topic
Day 1| DSA Fundamentals
Day 2| Time Complexity
Day 3| Space Complexity
Day 4| Auxiliary Space
Day 5| Case Analysis
Day 6| Recursion
