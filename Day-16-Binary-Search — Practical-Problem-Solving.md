DSA Day 16: Binary Search — Practical Problem Solving

📌 Overview

Today, I continued learning Data Structures and Algorithms (DSA) by practising Binary Search. I revised the fundamental concepts, studied the algorithm's implementation in Python, and analysed its time and space complexity.

🎯 Topics Covered

- Binary Search revision
- Searching for a target element in a sorted list
- Understanding "left", "right", and "mid"
- Using a "while" loop to implement Binary Search
- Updating search boundaries
- Analysing time and auxiliary space complexity
- Practising DSA multiple-choice questions

🔍 What Is Binary Search?

Binary Search is an efficient searching algorithm that repeatedly divides a sorted search space into halves to locate a target element.

Unlike Linear Search, which checks elements one by one, Binary Search eliminates approximately half of the remaining search space in each iteration.

Important: A standard Binary Search implementation requires sorted data.

⚙️ How Binary Search Works

1. Initialise "left" to "0".
2. Initialise "right" to "len(arr) - 1".
3. Calculate the middle index using "(left + right) // 2".
4. Compare the middle element with the target.
5. If both are equal, return the middle index.
6. If the middle element is smaller than the target, update "left = mid + 1".
7. If the middle element is larger than the target, update "right = mid - 1".
8. Repeat until the target is found or the search space becomes empty.

💻 Python Implementation

arr = [10, 20, 30, 40, 50, 60, 70]
target = 50

left = 0
right = len(arr) - 1
result = -1

while left <= right:
    mid = (left + right) // 2

    if arr[mid] == target:
        result = mid
        break
    elif arr[mid] < target:
        left = mid + 1
    else:
        right = mid - 1

print(result)

Output:

4

The target "50" is located at index "4". If the target is not found, the program returns "-1".

⏱️ Time and Space Complexity

Case| Complexity
Best-case time| O(1)
Average-case time| O(log n)
Worst-case time| O(log n)
Auxiliary space| O(1)

The iterative implementation uses constant auxiliary space because it requires only a fixed number of additional variables.

🧠 Key Learnings

- Binary Search is efficient for searching sorted data.
- The middle index helps eliminate unnecessary comparisons.
- Updating the search boundaries correctly is essential.
- "left = mid + 1" searches the right half.
- "right = mid - 1" searches the left half.
- The iterative Binary Search algorithm has O(log n) worst-case time complexity and O(1) auxiliary space complexity.

✅ Day 16 Progress

- Revised Binary Search fundamentals.
- Studied the Python implementation.
- Reviewed time and space complexity.
- Completed a five-question quiz with a score of 5/5.

🚀 Next Step

Continue practising Binary Search problems, including finding elements that are absent from a sorted list and understanding boundary conditions.

Consistency is the key to mastering DSA and preparing for technical placement interviews.
