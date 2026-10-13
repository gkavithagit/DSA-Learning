Day 13: Binary Search Practice

📌 Overview

Today, I revised Binary Search and strengthened my understanding of its working mechanism, time complexity, and implementation using Python.

📚 Topics Covered

- Revision of the Binary Search algorithm.
- Understanding the "low", "high", and "mid" variables.
- Searching for an element in a sorted array.
- Understanding how Binary Search eliminates half of the search space in each iteration.
- Comparing Linear Search and Binary Search.
- Analysing time and auxiliary space complexity.
- Solving multiple-choice questions to test conceptual understanding.

🔍 Linear Search vs Binary Search

Feature| Linear Search| Binary Search
Approach| Checks elements sequentially| Divides the search space in half
Requirement| Does not require sorted data| Standard implementation requires sorted data
Best-case time| O(1)| O(1)
Worst-case time| O(n)| O(log n)
Auxiliary space| O(1)| O(1) for iterative implementation

💻 Python Implementation

arr = [3, 8, 12, 17, 25, 31, 42]
target = 25

low = 0
high = len(arr) - 1

while low <= high:
    mid = (low + high) // 2

    if arr[mid] == target:
        print("Target found at index:", mid)
        break
    elif arr[mid] < target:
        low = mid + 1
    else:
        high = mid - 1
else:
    print("Target not found")

Output

Target found at index: 4

⏱️ Complexity Analysis

- Best-case time complexity: O(1)
- Worst-case time complexity: O(log n)
- Auxiliary space complexity: O(1)

🎯 Key Takeaways

- Binary Search works efficiently on sorted arrays.
- The middle element determines which half to search next.
- Updating "low" and "high" correctly is essential.
- Binary Search provides logarithmic time complexity.
- Understanding the algorithm's logic is more important than memorising its code.

📈 Learning Progress

Day 13 focused on strengthening my Binary Search fundamentals and applying them through Python implementation and complexity analysis.

Next Goal: Continue practising searching algorithms and solve more placement-oriented DSA problems.
